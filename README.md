# 📚 My Library

Personal reading locally → **http://localhost:9080**

## ➕ How to add a new book

1. Create a Books folder and drop the PDF into the `books/` folder (use a clean filename, e.g. `clean-code.pdf`)
2. Open `books.json` and add an entry:

```json
{
  "id": "clean-code",
  "title": "Clean Code",
  "author": "Robert C. Martin",
  "file": "books/clean-code.pdf",
  "cover": "",
  "tags": ["software engineering", "best practices"]
}
```


That's it — the book appears on the homepage automatically.

## 📱 Cross-device page sync

The reader saves your current page in the **URL hash** (e.g. `viewer.html?book=...#page=42`) and in `localStorage`.

To resume on another device, use the **🔗 Share** button in the toolbar — it copies a direct link to your current page. Open it on your phone or laptop and you'll land on the exact page.

## 🗂 Structure

```
index.html      ← Library homepage
viewer.html     ← Universal PDF reader
books.json      ← Book manifest (edit this to add books)
books/
  ddia.pdf
  ...
```
