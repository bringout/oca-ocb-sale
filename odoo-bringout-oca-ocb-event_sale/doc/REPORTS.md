# Reports

Report definitions and templates in event_sale.

```mermaid
classDiagram
    class EventSaleReport
    Model <|-- EventSaleReport
```

## Available Reports

### Analytical/Dashboard Reports
- **Revenues** (Analysis/Dashboard)


## Report Files

- **event_event_templates.xml** (XML template/definition)
- **event_sale_report.py** (Python logic)
- **event_sale_report_views.xml** (XML template/definition)
- **__init__.py** (Python logic)

## Notes
- Named reports above are accessible through Odoo's reporting menu
- Python files define report logic and data processing
- XML files contain report templates, definitions, and formatting
- Reports are integrated with Odoo's printing and email systems
