# SHEIN dataset: free samples for the US, UK, Germany and France (10,000 products each)

Free samples of **SHEIN product data**: 10,000 random products per country, each taken from a full snapshot of
that country's catalogue. Every product has its local price, crossed-out price and discount, full category path,
reviews and rating, colours, image URLs, seller store and creation date.

| Country | Snapshot | Products in the full catalogue | Currency |
|---|---|---|---|
| United States | 11 November 2026 | 21,389,348 | USD |
| United Kingdom | 17 October 2026 | 5,154,854 | GBP |
| Germany | 10 November 2026 | 3,123,472 | EUR |
| France | 10 November 2026 | 2,724,075 | EUR |

**Full catalogues** and **other SHEIN countries**:
**[cartpie.com/datasets/shein](https://cartpie.com/datasets/shein)**. Statistics from the full catalogues:
[SHEIN research on Cartpie](https://cartpie.com/research).

Also on Hugging Face ([US](https://huggingface.co/datasets/votiakov/shein-us-products-sample), [UK](https://huggingface.co/datasets/votiakov/shein-uk-products-sample), [Germany](https://huggingface.co/datasets/votiakov/shein-de-products-sample), [France](https://huggingface.co/datasets/votiakov/shein-fr-products-sample)) and Kaggle ([US](https://www.kaggle.com/datasets/votiakov/shein-us-products-sample), [UK](https://www.kaggle.com/datasets/votiakov/shein-uk-products-sample), [Germany](https://www.kaggle.com/datasets/votiakov/shein-de-products-sample), [France](https://www.kaggle.com/datasets/votiakov/shein-fr-products-sample)).

Made by [Andrii Votiakov](https://votiakov.com).

## Files

| File | Format | Rows |
|---|---|---|
| [`data/shein_us_sample_10k_2026-11-11.csv`](data/shein_us_sample_10k_2026-11-11.csv) | CSV (UTF-8, header; image URLs separated by `\|`) | 10,000 |
| [`data/shein_us_sample_10k_2026-11-11.parquet`](data/shein_us_sample_10k_2026-11-11.parquet) | Parquet (zstd) | 10,000 |
| [`data/shein_gb_sample_10k_2026-10-17.csv`](data/shein_gb_sample_10k_2026-10-17.csv) | CSV (UTF-8, header; image URLs separated by `\|`) | 10,000 |
| [`data/shein_gb_sample_10k_2026-10-17.parquet`](data/shein_gb_sample_10k_2026-10-17.parquet) | Parquet (zstd) | 10,000 |
| [`data/shein_de_sample_10k_2026-11-10.csv`](data/shein_de_sample_10k_2026-11-10.csv) | CSV (UTF-8, header; image URLs separated by `\|`) | 10,000 |
| [`data/shein_de_sample_10k_2026-11-10.parquet`](data/shein_de_sample_10k_2026-11-10.parquet) | Parquet (zstd) | 10,000 |
| [`data/shein_fr_sample_10k_2026-11-10.csv`](data/shein_fr_sample_10k_2026-11-10.csv) | CSV (UTF-8, header; image URLs separated by `\|`) | 10,000 |
| [`data/shein_fr_sample_10k_2026-11-10.parquet`](data/shein_fr_sample_10k_2026-11-10.parquet) | Parquet (zstd) | 10,000 |
| [`data/schema.json`](data/schema.json) | Field names, types and descriptions | |

## Preview

United States:

| Title | Price | Was | Off | Category | Reviews | Rating |
|---|---|---|---|---|---|---|
| Veilorie Plus Size Women Spring/Autumn Casual Solid Color Hi… | $25.07 | $37.19 | 33% | Plus Size Co-Ords | 37 | 4.62 |
| 1 Pair Adjustable Silicone Swim Training Hand Paddles, Unise… | $4.37 | $7.50 | 42% | Swimmer Fins | 44 | 4.84 |
| Plus Size Women Casual Round Neck Short Sleeve Cute Dachshun… | $6.63 | $13.28 | 50% | Women Tops | 161 | 4.60 |
| Woke Up Sexy As Hell Again T-Shirt Funny Saying Sarcastic T-… | $4.88 | $5.98 | 18% | Women T-Shirts | 900 | 4.76 |
| 1pc Elegant Style Oversized Rhinestone Bow Design Handmade F… | $4.60 | $5.80 | 21% | Women Brooch, Lapel Pin & Scarf Ring | 37 | 4.89 |

United Kingdom:

| Title | Price | Was | Off | Category | Reviews | Rating |
|---|---|---|---|---|---|---|
| 1pc Multi-Functional Clothes Hanger Stand, Garment Hanging R… | £19.48 | £24.28 | 20% | Coat Rack | 244 | 4.62 |
| 3pcs Letter Pendant Accessories, Straw Lid, Cup Name Tag, In… | £2.58 | £3.28 | 21% | Water Bottle & Cup Accessories | 93 | 4.98 |
| 4pcs/Set Gentle Style Y-Shaped Necklace Set, Pink Flower She… | £4.78 | £5.98 | 20% | Women Necklace Sets | 55 | 4.58 |
| SHEIN Unity Women Y2K Denim Crop Top, Music Festival Denim C… | £8.87 | £12.49 | 29% | Women Denim Tops | 176 | 4.77 |
| Normani Women's Fashionable Sexy Solid Color Backless Halter… | £17.49 | £22.49 | 22% | Women Mini Dresses | 117 | 4.67 |

Germany:

| Title | Price | Was | Off | Category | Reviews | Rating |
|---|---|---|---|---|---|---|
| SHEIN Newborn Baby Girl Cute Casual Yellow Cap Sleeve Knit B… | 8.96€ | 11.49€ | 22% | Baby Girls Bodysuits | 108 | 4.83 |
| Lyckli Maternity Two Pieces Suits | 25.27€ | 31.99€ | 21% | Maternity Two-piece Suits | 498 | 4.67 |
| YSTYLE Stretch Sofa Cover 1/2/3/4 Seater, Sofa Cover Non-Sli… | 23.48€ | 59.99€ | 61% | Sofa Slipcovers | 544 | 4.77 |
| SHEIN BAE Plus Size Polka Dot Beaded Halter Neck Tie Sexy Fl… | 11.69€ | 17.99€ | 35% | Plus Size Bikini Sets | 974 | 4.55 |
| SHEIN MOD Ditsy Floral Plaid Pattern Ruffle Hem Mini Halter… | 15.59€ | 23.99€ | 35% | Women Mini Dresses | 117 | 4.70 |

France:

| Title | Price | Was | Off | Category | Reviews | Rating |
|---|---|---|---|---|---|---|
| Aralina Curve Women Textured Fabric Detail One Piece Swimsui… | 12.59€ | 17.99€ | 30% | Plus Size One-Pieces | 625 | 4.68 |
| Uveous 13x4 13x6 Wear And Go Glueless Wigs, Pre-Plucked, Pre… | 27.44€ | 39.68€ | 31% | Human Lace Wigs | 30 | 4.86 |
| SHEIN Privé Plus Size Elegant Plush Printed Fitted Short A-L… | 15.50€ | 30.99€ | 50% | Plus Size Dresses | 371 | 4.88 |
| TaskSense Women's Fashionable Casual Tropical Cute Street St… | 14.69€ | 20.99€ | 30% | Women Short Dresses | 46 | 4.69 |
| Siren Gaze 100 Cotton Summer Women Embroidered Lace Trim Sho… | 9.44€ | 13.49€ | 30% | Women Blouses & Shirts | 335 | 4.62 |

## Quick start

```python
import pandas as pd
df = pd.read_parquet("data/shein_de_sample_10k_2026-11-10.parquet")
print(df.groupby("top_category")["price"].median().sort_values())
```

```sql
-- DuckDB: the same product priced in Germany and France
SELECT de.product_id, de.title, de.price AS price_de, fr.price AS price_fr
FROM 'data/shein_de_sample_10k_2026-11-10.parquet' de
JOIN 'data/shein_fr_sample_10k_2026-11-10.parquet' fr USING (product_id)
ORDER BY abs(de.price - fr.price) DESC;

-- The same product in the US and Germany, both in US dollars. The two samples share only a few products;
-- the full datasets share about 1.9 million.
SELECT us.product_id, us.title, us.price AS price_us_usd, de.price_usd AS price_de_usd
FROM 'data/shein_us_sample_10k_2026-11-11.parquet' us
JOIN 'data/shein_de_sample_10k_2026-11-10.parquet' de USING (product_id);
```

## Fields

| Field | Type | Description |
|---|---|---|
| `product_id` | string | SHEIN product ID (goods ID). Unique per row. The same ID is the same product in every country. |
| `sku` | string | SHEIN SKU code of this colour variant. |
| `spu` | string | SHEIN SPU code shared by all colour variants of a product. |
| `title` | string | Product title as shown to shoppers. |
| `product_url` | string | Product page on the country's SHEIN storefront. |
| `country` | string | ISO country code of the storefront, e.g. GB = United Kingdom, DE = Germany. |
| `currency` | string | ISO currency of the prices. |
| `price` | number | Selling price in local currency, as shown to shoppers (UK and EU: incl. VAT; US: before sales tax). |
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
| `stock_indicator` | integer | Stock as shown to shoppers: exact count below 10, 999 = 10 or more; empty when not reported. |
| `review_count` | integer | Number of reviews; 1001 means 1,000 or more. |
| `rating` | number | Average star rating (1–5); empty when the product has no reviews. |
| `color_count` | integer | Number of colour variants offered. |
| `image_url` | string | Main product image URL. |
| `image_urls` | list of strings | All product image URLs (in CSV: separated by '|'). |
| `image_count` | integer | Number of product images. |
| `seller_store_id` | string | ID of the seller storefront that lists the product. |
| `created_date` | date | Date the product was created. |
| `collected_at` | timestamp | When this record was collected, with its UTC offset. |

## Notes

- One row per product (colour variant). `product_id` is the same product in every SHEIN country, so country datasets join on it.
- Prices are what shoppers in each country see, in local currency: UK and EU prices include VAT, US prices are before sales tax.
- `stock_indicator` is empty for every product in the US snapshot.
- `review_count` is capped at 1001, which means 1,000 or more. `stock_indicator` is exact below 10; 999 means 10 or more; it is empty when not reported.
- `rating` is empty for products without reviews.
- Image URLs link to SHEIN's image CDN. No image files are included.
- Independent data. Not affiliated with, endorsed by or sponsored by SHEIN. SHEIN is a trademark of its owner.

## Terms

Free to use for evaluation, research and journalism, with attribution to
Cartpie ([cartpie.com](https://cartpie.com)). Not for resale or redistribution as a dataset.
For commercial use and the full data, get a licence at [cartpie.com/datasets/shein](https://cartpie.com/datasets/shein).
