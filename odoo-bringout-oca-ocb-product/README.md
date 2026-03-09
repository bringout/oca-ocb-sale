# Products & Pricelists


This is the base module for managing products and pricelists in Odoo.
========================================================================

Products support variants, different pricing methods, vendors information,
make to stock/order, different units of measure, packaging and properties.

Pricelists support:
-------------------
    * Multiple-level of discount (by product, category, quantities)
    * Compute price based on different criteria:
        * Other pricelist
        * Cost price
        * List price
        * Vendor price

Pricelists preferences by product and/or partners.

Print product labels with barcode.
    

## Installation

```bash
pip install odoo-bringout-oca-ocb-product
```

## Dependencies

- base
- mail
- uom

## Source

- Repository: https://github.com/OCA/OCB
- Branch: 19.0
- Path: addons/product

## License

This package preserves the original LGPL-3 license.
