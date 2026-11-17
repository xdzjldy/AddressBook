# AddressBook — Advanced Address Book System

A web-based address book built with **Flask (Python)** and **Bootstrap 5**, developed as a team assignment for the Software Engineering (FZU–MU) course.

## Features

- **Contact Management** — Add, list, and delete contacts. Bookmarked contacts are highlighted and pinned to the top of the list.
- **Bookmark Contacts** ⭐ — Mark important or frequently contacted people with one click; they stay on top for quick access.
- **Multiple Contact Methods** — Store phone numbers, emails, social media handles, addresses and more for a single contact (multi-line text field).
- **Excel Export** — Export every contact and all associated information to `.xlsx`. One row per contact, one column per information type (`Name`, `IsBookmarked`, `ContactMethods`).
- **Excel Import** — Upload a correctly formatted Excel file and all contacts are parsed and added to the address book automatically.

## Technology Stack

| Layer     | Technology                                      |
|-----------|--------------------------------------------------|
| Backend   | Python 3, Flask, Flask-SQLAlchemy (SQLite)       |
| Frontend  | HTML5, Bootstrap 5, Vanilla JavaScript           |
| Data      | Pandas, openpyxl / xlrd (Excel read & write)     |

## Getting Started

```bash
# 1. Install dependencies
pip install -r requirements.txt

# 2. Run the application
python app.py

# 3. Open in browser
# http://127.0.0.1:5000
```

The SQLite database (`instance/addressbook.db`) is created automatically on first run.

## Excel File Format

| Name (required) | IsBookmarked | ContactMethods                 |
|-----------------|--------------|--------------------------------|
| Alice           | Yes          | Phone:13800000000; Email:a@b.com |
| Bob             | No           | Phone:13900000000              |

## Team Members

| Member     | Contribution                                                     |
|------------|------------------------------------------------------------------|
| Sifan Wu   | Frontend UI (Bootstrap layout), bookmark interaction, HTML/JS    |
| Jingqi Tong| Backend Flask routes, database model, Excel import/export, docs  |
