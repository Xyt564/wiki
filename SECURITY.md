# Security — v1

**Version:** 1.0
**Last Updated:** February 2026

This document outlines **security considerations** for the Local Wiki application.

---

## 1. Offline Operation

* The Local Wiki runs **entirely on your machine**, with **no internet access required**.
* Notes, tags, and subjects are stored **locally in a JSON file** (`wiki.json`) inside the folder you specify.
* The application does **not send data to any server**, ensuring your knowledge stays private.

---

## 2. Data Storage

* All notes are saved in **plaintext JSON** by default.
* Exported files (`wiki_export.json`) are also **unencrypted JSON**.
* You are responsible for securing your folder and backups.

> ⚠️ Avoid storing sensitive information if the device or folder may be shared or exposed.

---

## 3. File Location & Permissions

* You must set your own `data_dir` in `wiki.py`.
* Ensure the folder permissions prevent unauthorized access, especially if using a shared or networked machine.
* The application will **create the folder automatically** if it doesn’t exist.

---

## 4. Dependencies

* `customtkinter` — for GUI rendering
* Python standard libraries for JSON handling

> Install dependencies via `pip install -r requirements.txt` from the official Python package repositories.
> Using only trusted sources reduces the risk of malicious packages.

---

## 5. Security Limitations

1. **Plaintext storage**: Notes are stored unencrypted. Anyone with access to the folder can read them.
2. **No authentication**: The app does not have login or access controls.
3. **Local-only**: Data is never transmitted online unless you manually move or share exported files.

> 🛡️ Security depends entirely on folder access and responsible handling of exported files.

---

## 6. Recommendations

* Regularly **backup your notes** by exporting JSON files.
* **Do not store sensitive personal or financial information** if other people can access your device.
* Keep your **Python environment and dependencies up to date**.
* Set **file/folder permissions** appropriately to prevent unauthorized access.

---

## 7. Future Updates

* This is **v1**, and will **only be updated upon request** or if a contributor submits security improvements.
* Any new release will explicitly note **changes to security practices**.

---

> **Summary:** Local Wiki is designed to be fully offline and private, but note security relies on folder access and responsible management of JSON files. Exported notes are plaintext and unencrypted.

---
