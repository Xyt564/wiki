# Local Wiki

A sleek, **dark-themed local wiki application** built with **CustomTkinter** for managing notes, tags, and subjects offline. Perfect for keeping track of knowledge, ideas, and references all in one place.

---

## Features

* **Save, delete, and edit notes** with a simple, intuitive interface.
* **Organize notes with tags** for easy searching.
* **Search by title or tag** to quickly find notes.
* **Export all notes** to a JSON file for backup or sharing.
* **Dark mode UI** with a modern, minimal design.
* Fully offline and lightweight.

---

## Installation

1. **Clone the repository**:

```bash
git clone https://github.com/Xyt564/wiki.git
```

```bash
cd wiki
```

2. **Install dependencies**:

```bash
pip install -r requirements.txt
```

> Only dependency: `customtkinter`

3. **Update your data folder path**:

Open `wiki.py` and locate the `data_dir` variable near the top:

```python
data_dir = "YOUR_FOLDER_LOCATION"
```

Change it to a folder on your system where you want your wiki data to be saved. For example:

```python
# Windows
data_dir = "C:/Users/YourName/Downloads/wiki"

# macOS/Linux
data_dir = "/Users/yourname/Downloads/wiki"
```

> The folder will be automatically created if it doesn’t exist.
> The app stores your notes in `wiki.json` inside this folder.

4. **Run the application**:

```bash
python wiki.py
```

---

## Usage

1. **Add a note**:

   * Enter a **title**, **tags** (comma-separated), and **content**, then click **Save**.

2. **Edit a note**:

   * Select a note from the list, make changes, and click **Save**.

3. **Delete a note**:

   * Select a note and click **Delete**.

4. **Search notes**:

   * Type a keyword in the search box to filter by **title or tag**.

5. **Export notes**:

   * Click **Export** to save all notes as `wiki_export.json` in your `data_dir`.

---

## File Structure

```
wiki/
├── wiki.py            # Main application code
├── requirements.txt   # Dependencies
└── wiki.json          # Automatically generated database file
```

* `wiki.json` stores all your notes in JSON format.
* `wiki_export.json` is created when you export your notes.

---

## Customization

* **Themes & Colors**: You can modify the colors or fonts in the top section of `wiki.py`:

```python
BG = "#1a1d23"          # Background
PANEL = "#22262e"       # Main panel
BUTTON_BG = "#6366f1"   # Button background
ACCENT = "#06b6d4"      # Highlight accent
TEXT = "#f8fafc"        # Text color
```

* **Window size**: Modify the geometry in `wiki.py`:

```python
root.geometry("1000x620")
```

---

## Contributing

Contributions are welcome! You can put in a request for me to:

* Add features (like Markdown support, images, or syncing).
* Improve UI/UX or accessibility.
* Optimize performance for large note databases.
* Fix bugs or improve stability.

> Please submit issues or pull requests through GitHub.

---

## License

This project is licensed under the **MIT License**, which is one of the most permissive and widely used open-source licenses.

### What the MIT License allows:

* **Free use**: You can use the software for personal, academic, or commercial purposes.
* **Modification**: You can change the code to suit your needs.
* **Distribution**: You can share the original or modified code freely.
* **Sublicensing**: You can include it in other projects, including proprietary ones.

### Conditions:

* You **must include the original copyright and license notice** in any copies or substantial portions of the software.
* The software is provided **“as-is”**, without warranty of any kind. The authors are not responsible for any damage or issues that arise from using it.

> In short: You can do almost anything with the code, just give credit and don’t expect a warranty.

---
