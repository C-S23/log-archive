# LOG-archive
### Log Archiver Tool - README

A shell script to compress logs from a specified directory into a `tar.gz` file, store it in an archive directory, and log the operation details.



#### Usage

./log_archiver.sh <log-directory> [archive-directory] [-v|--verbose]


- `<log-directory>`: Path to the directory containing logs (required).
- `[archive-directory]`: Output directory for archives (optional, defaults to `archives/`).
- `-v | --verbose`: Enable detailed output during archiving (optional).



#### Example
1. Basic usage:
   
   ./log_archiver.sh /path/to/logs
   
2. Specify a custom archive directory:
   
   ./log_archiver.sh /path/to/logs /path/to/archives
   
3. Enable verbose mode:
   
   ./log_archiver.sh /path/to/logs -v
   



#### Output
- Compressed File: Stored in the archive directory, e.g., `archives/logs_archive_YYYYMMDD_HHMMSS.tar.gz`.
- Log File: Details logged in `archives/archive_log.txt`.



#### Requirements
- `bash`
- `tar`



#### Notes
- Ensure the script has execute permissions:
  
  chmod +x log_archiver.sh
  
- For scheduled archiving, add it to a cron job.

Enjoy simplified log archiving! 😊
