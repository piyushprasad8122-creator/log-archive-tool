# Log Archive CLI Tool


A simple command-line tool to archive system logs by compressing them into a `.tar.gz` file with a timestamp.  
Useful for cleaning up old logs while keeping them available for future reference.


---


## Features


- Accepts a log directory as an argument
- Compresses logs into a timestamped `.tar.gz` file
- Stores archives in a separate directory
- Logs archive date and time


---


## Usage


Make the script executable:


```bash
chmod +x log-archive

Run the tool:

./log-archive <log-directory>

Example:

./log-archive /var/log
Archive Format
logs_archive_YYYYMMDD_HHMMSS.tar.gz

Example:

logs_archive_20240816_100648.tar.gz
Requirements

Linux / Unix-based system

Bash

tar utility

Future Improvements

Cron job automation

Email notifications

Upload archives to cloud storage (AWS S3)

Delete old logs after archiving

Author

Piyush



---


## 3️⃣ `.gitignore` (important)


Create a file named **`.gitignore`** and paste this:


```text
log-archives/
*.tar.gz
