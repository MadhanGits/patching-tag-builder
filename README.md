# SQL Patching Tag Builder 🛠️

A simple, elegant web tool to dynamically generate standardized patching tags and plain-English descriptions for SQL Server maintenance scheduling.
This tool helps you generate a patching schedule tag that specifies the method, type, week, day, and time block for SQL Server patching. It also allows you to provide the application name to specify which application the tag corresponds to.

# How to Use
**Patch Method:**

Select AU for Automatic Update (this is the default method).

**Patch Type:**

Select SQL (this is the patch type we are applying).

**Patch Week:**

0: This is the week of the 2nd Tuesday of every month. Typically used for DEV/TEST devices only.

1: This is the production patch week, starting from Day 0 to Day 6 (the week immediately following the 2nd Tuesday of the month).

2: This is the production patch week, starting from Day 7 to Day 12 (the week after the first production patch week).

**Maintenance Day:**

Select the day of the week when the patching is scheduled to take place.

For DEV/TEST patch weeks (week 0), you can’t select Monday or Tuesday.

For production patch weeks (week 1 and 2), all days of the week are available.

**Time Block:**

Choose the time window for when the patching should occur. 
Time blocks range from late night (12:01 AM) to late evening (11:59 PM).

**Application Name:**

Enter the application name (e.g., NAW) for better identification of the patching tag.

---

# Understanding the Patch Week Selection

  - Week 0: This is the week of the 2nd Tuesday of the month (for testing/dev purposes).

  - Week 1: This is the production patch week, immediately after the 2nd Tuesday.

  - Week 2: This is the next production patch week, starting 7 days after Week 1.

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
<< AU-SQL-0-WE-0001-0400-MSFT >>
```

**Description:**  
Automatic patching for SQL will be scheduled during the week of the 2nd Tuesday of the month (for Dev/Test), on Wednesday, between 12:01 AM to 4:00 AM, for application MSFT.

---

## 💡 Use Cases

- **DBAs** scheduling SQL patching windows
- **IT Teams** coordinating Dev/Test and Production maintenance
- **Change Management** documentation

---

## 🛠️ Future Customization Ideas

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
