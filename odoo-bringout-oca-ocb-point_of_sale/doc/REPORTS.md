# Reports

Report definitions and templates in point_of_sale.

```mermaid
classDiagram
    class PosOrderReport
    Model <|-- PosOrderReport
    class PosInvoiceReport
    AbstractModel <|-- PosInvoiceReport
```

## Available Reports

No named reports found in XML files.


## Report Files

- **__init__.py** (Python logic)
- **pos_invoice.py** (Python logic)
- **pos_order_report.py** (Python logic)

## Notes
- Named reports above are accessible through Odoo's reporting menu
- Python files define report logic and data processing
- XML files contain report templates, definitions, and formatting
- Reports are integrated with Odoo's printing and email systems
