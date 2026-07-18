= Engineering Documentation Standards

This guide defines formatting and metadata requirements for all developer-facing documentation.

== Typography and Highlights

* *UI Components:* Use bold for buttons, menus, and interface elements (e.g., *Submit*).
* `Paths & Variables:` Use backticks for file paths, folder structures, and environmental variables (e.g., `src/config.json`).
* _Emphasis:_ Use italics for key terms or conceptual labels.

== Code Block Standards

Always specify the language in the opening fence to ensure correct syntax highlighting.

[source,python]
----
def calculate_uptime(total, downtime):
    """Computes operational availability percentage."""
    if total == 0:
        return 0.0
    return ((total - downtime) / total) * 100
----

== Review Checklist

Before merging documentation updates, verify the following:

* *Links:* Use relative paths for all internal links (no absolute URLs).
* *Tables:* Verify all tables contain explicit, properly formatted header rows.
* *Media:* Use compressed formats (`.webp` or `.png`) for all image assets.
* *Clarity:* Keep content direct; avoid filler words and unnecessary process background.
