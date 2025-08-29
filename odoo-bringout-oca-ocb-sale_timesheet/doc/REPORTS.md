# Reports

Report definitions and templates in sale_timesheet.

```mermaid
classDiagram
    class TimesheetsAnalysisReport
    Model <|-- TimesheetsAnalysisReport
```

## Available Reports

### PDF/Document Reports
- **Timesheets** (PDF/Print)
- **Timesheets** (PDF/Print)


## Report Files

- **__init__.py** (Python logic)
- **report_timesheet_templates.xml** (XML template/definition)
- **timesheets_analysis_report.py** (Python logic)
- **timesheets_analysis_views.xml** (XML template/definition)

## Notes
- Named reports above are accessible through Odoo's reporting menu
- Python files define report logic and data processing
- XML files contain report templates, definitions, and formatting
- Reports are integrated with Odoo's printing and email systems
