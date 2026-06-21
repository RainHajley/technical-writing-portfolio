# Engineering Documentation Markdown Styling Standards

This internal reference guide defines the code-formatting rules, typographical standards, and metadata conventions required for all developer-facing documentation.

---

## Typography and Highlights

* **UI Components:** Use bolding for clickable buttons, menus, and user interface elements (e.g., "Click **Submit**").
* **File Paths and Variables:** Wrap system properties, relative folder structures, and environmental variables in backticks (e.g., `src/main/resources/config.json`).

---

## Code Block Standards

All sample source blocks must specify the exact rendering language in the opening fence to guarantee accurate syntax highlighting.

```python
def calculate_system_uptime(total_seconds, downtime_seconds):
    """Computes operational availability percentage."""
    if total_seconds == 0:
        return 0.0
    return ((total_seconds - downtime_seconds) / total_seconds) * 100
```

---

## Review Checklist

- [ ] Verify that all markdown links point to relative directory items rather than absolute localhost URLs.
- [ ] Confirm all tables contain explicit header rows.
- [ ] Validate that image assets utilize lightweight compressed media formats (`.webp` or `.png`).
