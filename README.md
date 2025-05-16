# 📥 Gmail Invoice Data Extractor

A Python-based tool to automatically extract and organize invoice data from your Gmail inbox. Designed for finance teams, freelancers, and small businesses, it eliminates the need for manual data entry by scanning emails and attachments for relevant invoice information.

---

## ✨ Features

- 🔐 **Secure Gmail Access**: Uses OAuth2 for safe, user-authorized access to Gmail.
- 📑 **Invoice Detection**: Identifies and filters invoice emails based on sender, subject, or attachment type.
- 📦 **Data Extraction**: Parses key fields like vendor, date, amount, and invoice number from both email body and attachments (PDF, etc.).
- 📊 **Exportable Data**: Outputs data into CSV or integrates easily into database systems.
- 🔄 **Customizable Parsing**: Modular structure allows adaptation for different invoice formats.
- ⚙️ **CLI-Based Workflow**: Simple, interactive command-line interface for ease of use.

---

## 🛠️ Tech Stack

- **Python 3**
- **Gmail API + OAuth2**
- **PDF Parsers**: `PyPDF2`, `pdfplumber`
- **Data Handling**: `pandas`
- **Worqhat APIs` (optional integrations)

---

## 🚀 Getting Started

### Prerequisites

- Python 3.7+
- Google Cloud Project with Gmail API enabled
- Gmail account with invoice-related emails

### Installation

```bash
git clone https://github.com/Manandadoo/Gmail-Invoice-Data-Extractor.git
cd Gmail-Invoice-Data-Extractor
pip install -r requirements.txt
```

### Setup Gmail API

1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Enable the **Gmail API**
3. Create OAuth2 credentials (Desktop Application)
4. Download `credentials.json` and place it in the project root

### Run the Extractor

```bash
python main.py
```

Follow the on-screen prompts for authentication and Gmail access.

---

## ⚙️ Customization

- **Filter rules**: Customize sender, subject, and label filters in `main.py`
- **Parsing logic**: Extend or adjust parsing in the `invoice_parser/` module
- **Storage format**: Modify export settings to save as CSV, JSON, or into a database

---

## 📌 Notes

- This tool only reads invoice-related emails. It does **not** send, delete, or modify any email content.
- OAuth credentials are stored locally for re-authentication.
- For production use, consider moving credentials and tokens into secure storage.

---

## 🔗 Resources

- [Gmail API Python Quickstart](https://developers.google.com/gmail/api/quickstart/python)
- [Google OAuth2 Documentation](https://developers.google.com/identity/protocols/oauth2)

---
