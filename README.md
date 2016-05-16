# Shopify to PowerReviews order feed converter
Converts Shopify order feed xml to PowerReviews order feed csv.

## Usage
```sh
shopify_pwr_order_feed/convert -h <shopify_feed_url> [-u <username>] [-p <password>] [-m <path_to_map_file>] > pwr-order-feed.csv
```
## Page id map
Page ids are a nececary part of PowerReviews order csv, since they cannot be found in Shopify order feed, `page-id-map.json` must be created.

It maps Shopify product SKU to PowerReviews page id:
```json
{
  "product-sku": "page-id"
}
```
