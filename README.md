# Log Archive CLI Tool


A Bash-based command-line tool that archives system logs by compressing them into timestamped `.tar.gz` files.  
This project is built as part of the **roadmap.sh Log Archive Tool project** and fulfills all the required objectives.


🔗 **Project Reference (Completed):**  
https://roadmap.sh/projects/log-archive-tool


---


## ✅ Project Status


✔️ This project has been **successfully completed** according to the requirements defined on **roadmap.sh**.  
✔️ All core features and expected behaviors are implemented and tested.


---


## 📌 Project Overview


On Unix/Linux systems, logs are commonly stored in `/var/log`.  
Over time, these logs can grow large and clutter the system.


This tool helps by:
- Archiving logs on demand
- Compressing them efficiently
- Storing them in a separate directory
- Keeping a record of archive operations


---


## ✨ Features


- Accepts a log directory as a command-line argument
- Compresses logs into a `.tar.gz` archive
- Uses timestamp-based archive naming
- Stores archives in a dedicated directory
- Logs the date and time of each archive operation
- Lightweight and easy-to-use CLI tool


---


## 📂 Project Structure



log-archive-tool/
├── log-archive
├── README.md
├── .gitignore
└── screenshots/



---


## ⚙️ Requirements


- Linux / Unix-based system
- Bash shell
- `tar` utility


---


## 🚀 Usage


### 1. Make the script executable


```bash
chmod +x log-archive
2. Run the tool
./log-archive <log-directory>
Example
./log-archive /var/log
🗂️ Archive Format

Archives are created using the following naming convention:

logs_archive_YYYYMMDD_HHMMSS.tar.gz

Example:

logs_archive_20240816_100648.tar.gz
🖼️ Screenshots
Running the tool
<img src="screenshots/run-command.png" width="700">
Generated archive files
<img src="screenshots/archive-files.png" width="700">
Archive history log
<img src="screenshots/archive-log.png" width="700">
📝 Archive Log

Each time the tool runs, it records the archive activity in:

~/log-archives/archive.log

Example entry:

Archived /var/log on Fri Aug 16 10:06:48 IST 2024
🔒 Git Ignore Rules

The following files and folders are excluded from version control:

log-archives/

*.tar.gz

This ensures the repository remains clean and lightweight.

🔮 Future Enhancements

Automate archiving using cron jobs

Email notifications after archive completion

Upload archives to cloud storage (AWS S3)

Automatically remove old logs after archiving

Add compression level options

👤 Author

Piyush

📄 License

This project is open-source and created for learning, practice, and portfolio purposes.
