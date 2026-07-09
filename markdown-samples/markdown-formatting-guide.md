# Engineering Documentation Standards

This guide defines the formatting and metadata requirements for all developer-facing documentation.

## Typography and Highlights

* **UI Components**: Use bold for buttons, menus, and interface elements (e.g., **Submit**).
* **Paths & Variables**: Use backticks for file paths, folder structures, and environmental variables (e.g., `src/config.json`).
* *Emphasis*: Use italics for key terms or conceptual labels.

## Code Block Standards

Always specify the language in the opening fence to enable correct syntax highlighting.

### Example

```python
def calculate_uptime(total, downtime):
    """Computes operational availability percentage."""
    if total == 0:
        return 0.0
    return ((total - downtime) / total) * 100
```

## Review Checklist

Before merging any documentation updates, verify the following:

- [ ] **Links**: All internal links use relative paths rather than absolute URLs.
- [ ] **Tables**: All tables contain explicit, properly formatted header rows.
- [ ] **Media**: All image assets use compressed formats (`.webp` or `.png`).
- [ ] **Clarity**: Ensure the tone is direct—avoid filler words and unnecessary process explanations.
