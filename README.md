# RealEstate_CRM
Real Estate Crm open source
# 🏢 Look-Out CRM & Invoice Manager (Python Desktop App)

A complete desktop-based CRM + Invoice Management system with backup, lead tracking, WhatsApp/email integration, task calendar, chart reporting, invoice PDF/HTML generation, and auto backup.

## ✅ Features

- Lead manager (Name, Phone, Email, Property, Notes, Follow-up)
- Tagging system
- PDF export and printing
- WhatsApp & Email integration
- Daily follow-up and reminders
- Task calendar with highlighting and categories
- Invoice generation (Classic / Modern style)
- Auto-fill invoice based on previous clients
- Backup & restore
- Beautiful GUI (Tkinter-based)
- Works fully **offline**

---

## 📦 Requirements

Python 3.8 or later

Install dependencies using:

```bash
pip install -r requirements.txt
Or manually:

bash
Copy
Edit
pip install tkcalendar openpyxl reportlab matplotlib
💻 How to Run
🪟 On Windows
Download or clone this repo:

bash
Copy
Edit
git clone https://github.com/your-username/lookout-crm.git
cd lookout-crm
Run the app:

bash
Copy
Edit
python main.py
(Optional) Convert to .exe using pyinstaller:

bash
Copy
Edit
pip install pyinstaller
pyinstaller --noconfirm --onefile --windowed main.py
🐧 On Linux (Ubuntu/Debian)
Install required packages:

bash
Copy
Edit
sudo apt update
sudo apt install python3-tk python3-pip
pip3 install tkcalendar openpyxl reportlab matplotlib
Run:

bash
Copy
Edit
python3 main.py
(Optional) Add desktop shortcut or .desktop launcher.

📱 On Android (via Termux + X11)
Install Termux & XServer XSDL from Play Store.

In Termux:

bash
Copy
Edit
pkg update
pkg install x11-repo
pkg install python tk
pip install tkcalendar openpyxl reportlab matplotlib
export DISPLAY=:0
python main.py
Start XServer XSDL app and wait for connection.

⚠️ Some features (PDF printing, file dialogs) may be limited in mobile environments.

📁 Files Structure
bash
Copy
Edit
📁 lookout-crm/
│
├── main.py                # Main application file
├── real_estate_leads.xlsx # Auto-created for lead storage
├── invoices.xlsx          # Auto-created for invoice records
├── tasks.txt              # Stores calendar tasks
├── tags.txt               # Stores user-created tags
├── backups/               # Excel file auto-backups
├── logo.png               # Your company logo (optional)
├── invoice.pdf            # Latest invoice PDF
├── invoice.html           # Latest invoice HTML
└── requirements.txt       # Python dependencies
🧠 Smart Tips
Logo: Place logo.png in root folder to include it on invoices.

WhatsApp: Valid local numbers like 03001234567 are auto-converted to +923001234567.

Invoice PDF/HTML auto-opens on generation.

Auto-backup is created every time you add/update leads.
