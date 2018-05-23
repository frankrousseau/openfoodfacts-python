# Open Food Facts client for your Python applications and scripts
===================================
![Open Food Facts](https://static.openfoodfacts.org/images/misc/openfoodfacts-logo-en-178x150.png)

## What is Open Food Facts?
### A food products database

Open Food Facts is a database of food products with ingredients, allergens, nutrition facts and all the tidbits of information we can find on product labels. 

### Made by everyone

Open Food Facts is a non-profit association of volunteers.
1800+ contributors like you have added 43 000+ products from 150 countries using our Android, iPhone or Windows Phone app or their camera to scan barcodes and upload pictures of products and their labels.

### For everyone

Data about food is of public interest and has to be open. The complete database is published as open data and can be reused by anyone and for any use. Check-out the cool reuses or make your own!
- <https://world.openfoodfacts.org>

## Status

[![Project Status](http://opensource.box.com/badges/active.svg)](http://opensource.box.com/badges)
[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/openfoodfacts/openfoodfacts-python.svg)](http://isitmaintained.com/project/openfoodfacts/openfoodfacts-python.svg "Average time to resolve an issue")
[![Percentage of issues still open](http://isitmaintained.com/badge/open/openfoodfacts/openfoodfacts-python.svg)](http://isitmaintained.com/project/openfoodfacts/openfoodfacts-python.svg "Percentage of issues still open")

## Contributing

The project is initially started by [](https://github.com/), other contributors include:
- [Pierre Slamich](https://github.com/teolemon)

## Copyright and License

    Copyright 2016 Open Food Facts

- [License](./LICENSE)

## Installation

    sudo pip install git+https://github.com/openfoodfacts/openfoodfacts-python

or:

    git clone https://github.com/openfoodfacts/openfoodfacts-python
    cd openfoodfacts-python
    sudo python setup.py install

## Docs

### Example Usage

*Query a Facet*

```python
brands = openfoodfacts.facets.get_brands()
```

*Basic Search*

```python
search_result = openfoodfacts.products.search(query)
```

*Add a new product.*

```python
status_code = openfoodfacts.products.add_new_product({
  'code': barcode,
  'user_id'  : myUsername,
  'password'  : myPassword,
  'product_name' : myProduct,
  'stores'  : store,
  'brands': brand,
  'packaging': packaging
})
```

To see all possible capabilities, check out the [usage guide](./docs/Usage.md).