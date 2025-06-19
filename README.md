# WikiAtHome

**Convert German Wikipedia Markdown links to Obsidian wikilinks – with optional folders, titles, and footnote support.**

---

## ✨ Features

This Obsidian plugin scans your Markdown notes for links to  Wikipedia (e.g. `https://de.wikipedia.org/wiki/...`) and converts them into Obsidian- internal links.

For example:

[Freistaat](https://de.wikipedia.org/wiki/Freistaat_\(Republik\) "Freistaat (Republik)")

…becomes:

[[Clippings/Freistaat (Republik) – Wikipedia|Freistaat]]


Supports:
- Escaped parentheses and unicode characters
- Footnotes like `[^1]`, which are preserved during replacement
- Custom folder prefix (e.g., `Clippings`) or none
- Custom title suffix (e.g., `– Wikipedia`) or none
- Custom wikilink (for example, https://de.wikipedia.org can and has to be changed to https://en.wikipedia.org in the Settings when converting English Wikipedia articles.)

---

## 🔧 Settings

You can configure:

- **Folder Prefix**: The folder where your wikilinks should point, e.g. `Clippings/`. Leave empty for no folder.
- **Title Suffix**: A custom suffix to append to the page title (e.g. ` – Wikipedia`). Leave empty to skip.
- **Custom wikilink**: Support for articles in different languages. "https://de.wikipedia.org" can and has to be changed to https://en.wikipedia.org in the Settings when converting English Wikipedia articles.


Go to **Settings → WikiAtHome Plugin** to set these values.

---
## Usage 

There is currently one way of running the plugin:

### ⌨️ Command Palette

Use the command palette (`Cmd/Ctrl+P`) and search for:

> `Convert Wikipedia links in current file`

This will run the conversion **only on the currently opened note**.

---

## 🧪 Example

Input:

```markdown
[Freistaat](https://de.wikipedia.org/wiki/Freistaat_%28Republik%29 "Freistaat (Republik)") [^1]
Output (default settings):

[[Clippings/Freistaat (Republik) – Wikipedia|Freistaat]] [^1]
