# SQL Patching Tag Builder 🛠️

A simple, elegant web tool to dynamically generate standardized patching tags and plain-English descriptions for SQL Server maintenance scheduling.

---

## 🚀 Features

- Generate SQL patching tags based on:
  - Patch Method
  - Patch Type
  - Patch Week (Dev/Test or Prod)
  - Maintenance Day
  - Time Block
  - Optional Application Name
- Automatically updates the tag and human-readable summary
- Responsive design with clean UI and focus states
- Copy-to-clipboard functionality for easy tag usage

---

## 🖼️ Preview

![image](https://github.com/user-attachments/assets/e04f7526-2006-4fff-90f2-be413cb611af)

---

## 📦 Getting Started

### 🔧 Prerequisites
No installation needed — just a modern browser (Chrome, Edge, Firefox, Safari).

### 🧪 Run Locally
```bash
git clone https://github.com/MadhanGits/patching-tag-builder.git
cd sql-patching-tag-builder
open index.html
```

Or simply open `index.html` in your browser.

---

## 📋 Example Tag

```
<< AU-SQL-1-WE-1201-1600-MSFT >>
```

**Description:**  
Automatic patching for SQL will be scheduled during the week of the 2nd Tuesday of the month (for Dev/Test), on Wednesday, between 12:01 AM to 4:00 AM.

---

## 💡 Use Cases

- **DBAs** scheduling SQL patching windows
- **IT Teams** coordinating Dev/Test and Production maintenance
- **Change Management** documentation

---

## 🛠️ Customization Ideas

- Add support for more patch types (e.g., OS, App)
- Persist settings using `localStorage`
- Export tags to CSV
- Mobile-friendly improvements
- Dark mode toggle

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to change.

---

## 📄 License

MIT License

---

## 🙋‍♂️ Author

Made with ❤️ by [MadhanGits]  
Connect with me on [LinkedIn](https://www.linkedin.com/in/madhanakkaldevi/))
