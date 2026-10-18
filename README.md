# SHEIN dataset: 10,000 UK products (free sample)

A free sample of **SHEIN product data**: 10,000 random products from SHEIN's United Kingdom catalogue,
taken from a full snapshot of **5,154,854 products** on 17 October 2026. Every product has its price in GBP,
crossed-out price and discount, full category path, stock, reviews and rating, colours, image URLs, seller
store and creation date.

**Full catalogues** (5M+ products per country), **daily feeds**, **price history** and **other SHEIN countries**:
**[votiakov.com/shein-data](https://votiakov.com/shein-data/)**. Free report on what the data shows:
[SHEIN by the numbers, UK, October 2026 (PDF)](https://votiakov.com/reports/shein-by-the-numbers-uk-2026-10.pdf).

Also on [Hugging Face](https://huggingface.co/datasets/votiakov/shein-uk-products-sample) and [Kaggle](https://www.kaggle.com/datasets/votiakov/shein-uk-products-sample).

## Files

| File | Format | Rows |
|---|---|---|
| [`data/shein_gb_sample_10k_2026-10-17.csv`](data/shein_gb_sample_10k_2026-10-17.csv) | CSV (UTF-8, header; image URLs separated by `\|`) | 10,000 |
| [`data/shein_gb_sample_10k_2026-10-17.parquet`](data/shein_gb_sample_10k_2026-10-17.parquet) | Parquet (zstd) | 10,000 |
| [`data/schema.json`](data/schema.json) | Field names, types and descriptions | |

## Preview

| Title | Price | Was | Off | Category | Reviews | Rating |
|---|---|---|---|---|---|---|
| 1pc Multi-Functional Clothes Hanger Stand, Garment Hanging R… | £19.48 | £24.28 | 20% | Coat Rack | 244 | 4.62 |
| 3pcs Letter Pendant Accessories, Straw Lid, Cup Name Tag, In… | £2.58 | £3.28 | 21% | Water Bottle & Cup Accessories | 93 | 4.98 |
| 4pcs/Set Gentle Style Y-Shaped Necklace Set, Pink Flower She… | £4.78 | £5.98 | 20% | Women Necklace Sets | 55 | 4.58 |
| SHEIN Unity Women Y2K Denim Crop Top, Music Festival Denim C… | £8.87 | £12.49 | 29% | Women Denim Tops | 176 | 4.77 |
| Normani Women's Fashionable Sexy Solid Color Backless Halter… | £17.49 | £22.49 | 22% | Women Mini Dresses | 117 | 4.67 |

## Quick start

```python
import pandas as pd
df = pd.read_parquet("data/shein_gb_sample_10k_2026-10-17.parquet")
print(df.groupby("top_category")["price"].median().sort_values())
```

```sql
-- DuckDB
SELECT top_category, count(*) AS products, median(price) AS median_price, avg(discount_pct) AS avg_discount
FROM 'data/shein_gb_sample_10k_2026-10-17.parquet'
GROUP BY 1 ORDER BY products DESC;
```

## Fields

| Field | Type | Description |
|---|---|---|
| `product_id` | string | SHEIN product ID (goods ID). Unique per row. The same ID is the same product in every country. |
| `sku` | string | SHEIN SKU code of this colour variant. |
| `spu` | string | SHEIN SPU code shared by all colour variants of a product. |
| `title` | string | Product title as shown to shoppers. |
| `product_url` | string | Product page on the country's SHEIN storefront. |
| `country` | string | ISO country code of the storefront (GB = United Kingdom). |
| `currency` | string | ISO currency of the prices. |
| `price` | number | Selling price in local currency, as shown to shoppers (UK: incl. VAT). |
| `price_display` | string | Selling price as displayed, with currency symbol. |
| `original_price` | number | Crossed-out (reference) price in local currency. |
| `original_price_display` | string | Crossed-out price as displayed. |
| `discount_pct` | number | 1 - price / original_price, rounded to 4 decimals; 0 when there is no crossed-out price above the price. |
| `price_usd` | number | Selling price converted to US dollars. |
| `top_category` | string | Top-level category name, e.g. Women Apparel. |
| `category` | string | Leaf category name, e.g. Women Mini Dresses. |
| `category_path` | string | Full category path from top level to leaf, separated by ' > '. |
| `category_id` | string | Leaf category ID. |
| `in_stock` | boolean | False when the product is shown as sold out. |
| `stock_indicator` | integer | Stock as shown to shoppers: exact count below 10, 999 = 10 or more. |
| `review_count` | integer | Number of reviews; 1001 means 1,000 or more. |
| `rating` | number | Average star rating (1–5); empty when the product has no reviews. |
| `color_count` | integer | Number of colour variants offered. |
| `image_url` | string | Main product image URL. |
| `image_urls` | list of strings | All product image URLs (in CSV: separated by '|'). |
| `image_count` | integer | Number of product images. |
| `seller_store_id` | string | ID of the seller storefront that lists the product. |
| `created_date` | date | Date the product was created. |
| `collected_at` | timestamp | When this record was collected (UTC). |

## Notes

- One row per product (colour variant). `product_id` is the same product in every SHEIN country, so country datasets join on it.
- Prices are what UK shoppers see, in GBP including VAT.
- `review_count` is capped at 1001, which means 1,000 or more. `stock_indicator` is exact below 10; 999 means 10 or more.
- `rating` is empty for products without reviews.
- Image URLs link to SHEIN's image CDN. No image files are included.
- Independent data. Not affiliated with, endorsed by or sponsored by SHEIN. SHEIN is a trademark of its owner.

## Terms

Free to use for evaluation, research and journalism, with attribution to
[votiakov.com/shein-data](https://votiakov.com/shein-data/). Not for resale or redistribution as a dataset.
For commercial use and the full data, get a licence at [votiakov.com/shein-data](https://votiakov.com/shein-data/).
