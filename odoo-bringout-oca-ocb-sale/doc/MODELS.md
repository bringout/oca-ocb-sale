# Models

Detected core models and extensions in sale.

```mermaid
classDiagram
    class account_move
    class sale_order
    class sale_order_line
    class account_analytic_applicability
    class account_analytic_line
    class account_move_line
    class analytic_mixin
    class crm_team
    class payment_provider
    class payment_transaction
    class product_attribute_custom_value
    class product_packaging
    class product_product
    class product_template
    class res_company
    class res_config_settings
    class res_partner
    class utm_campaign
    class res_company
    sale_order --> res_company : company_id (Many2one)
    class res_partner
    sale_order --> res_partner : partner_id (Many2one)
    class res_partner
    sale_order --> res_partner : partner_invoice_id (Many2one)
    class res_partner
    sale_order --> res_partner : partner_shipping_id (Many2one)
    class account_fiscal_position
    sale_order --> account_fiscal_position : fiscal_position_id (Many2one)
    class account_payment_term
    sale_order --> account_payment_term : payment_term_id (Many2one)
    class product_pricelist
    sale_order --> product_pricelist : pricelist_id (Many2one)
    class res_users
    sale_order --> res_users : user_id (Many2one)
    class crm_team
    sale_order --> crm_team : team_id (Many2one)
    class sale_order_line
    sale_order --> sale_order_line : order_line (One2many)
    class account_move
    sale_order --> account_move : invoice_ids (Many2many)
    class payment_transaction
    sale_order --> payment_transaction : transaction_ids (Many2many)
    class payment_transaction
    sale_order --> payment_transaction : authorized_transaction_ids (Many2many)
    class account_analytic_account
    sale_order --> account_analytic_account : analytic_account_id (Many2one)
    class crm_tag
    sale_order --> crm_tag : tag_ids (Many2many)
    class res_country
    sale_order --> res_country : tax_country_id (Many2one)
    class sale_order
    sale_order_line --> sale_order : order_id (Many2one)
    class product_product
    sale_order_line --> product_product : product_id (Many2one)
    class product_template
    sale_order_line --> product_template : product_template_id (Many2one)
    class product_attribute_custom_value
    sale_order_line --> product_attribute_custom_value : product_custom_attribute_value_ids (One2many)
    class product_template_attribute_value
    sale_order_line --> product_template_attribute_value : product_no_variant_attribute_value_ids (Many2many)
    class uom_uom
    sale_order_line --> uom_uom : product_uom (Many2one)
    class account_tax
    sale_order_line --> account_tax : tax_id (Many2many)
    class product_pricelist_item
    sale_order_line --> product_pricelist_item : pricelist_item_id (Many2one)
    class product_packaging
    sale_order_line --> product_packaging : product_packaging_id (Many2one)
    class account_analytic_line
    sale_order_line --> account_analytic_line : analytic_line_ids (One2many)
    class account_move_line
    sale_order_line --> account_move_line : invoice_lines (Many2many)
    class sale_order
    res_partner --> sale_order : sale_order_ids (One2many)
    class res_company
    utm_campaign --> res_company : company_id (Many2one)
    class res_currency
    utm_campaign --> res_currency : currency_id (Many2one)
    class sale_order
    payment_transaction --> sale_order : sale_order_ids (Many2many)
    class sale_order_line
    product_attribute_custom_value --> sale_order_line : sale_order_line_id (Many2one)
    class sale_order_line
    account_move_line --> sale_order_line : sale_line_ids (Many2many)
    class sale_order_line
    account_analytic_line --> sale_order_line : so_line (Many2one)
    class product_product
    res_config_settings --> product_product : deposit_default_product_id (Many2one)
    class mail_template
    res_config_settings --> mail_template : invoice_mail_template_id (Many2one)
    class crm_team
    account_move --> crm_team : team_id (Many2one)
```

Notes
- Classes show model technical names; fields omitted for brevity.
- Items listed under _inherit are extensions of existing models.
