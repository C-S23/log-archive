# LOG-archive
### Log Archiver Tool - README

A shell script to compress logs from a specified directory into a `tar.gz` file, store it in an archive directory, and log the operation details.

#### Usage in Linux machines:
Step 1: Download the Script

    git clone https://github.com/username/repository-name.git 
    cd repository-name

Make the script executable:

    chmod +x log_archiver.sh

Step 2: Run the Script

Run the script with the required arguments:

./log_archiver.sh <log-directory>

For example:

    ./log_archiver.sh /var/logs

one can even give optional arguments:

Specify an Archive Directory:

    ./log_archiver.sh /path/to/logs /path/to/archives

Enable Verbose Mode:

    ./log_archiver.sh /path/to/logs -v

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

#### Note:
- Ensure the script has execute permissions:
  
      chmod +x log_archiver.sh
  
- (if required) for scheduled job add script with cron job. [whats cron job?](https://phoenixnap.com/kb/set-up-cron-job-linux)
#### Project Link

For more details, visit the project page: [Log Archiver Tool](https://roadmap.sh/projects/log-archive-tool)
