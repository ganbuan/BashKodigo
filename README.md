# BashKodigo
Cheat sheet for common Bash commands 

## Basic Commands

**echo**: Output any provided text

**whoami**: Display current logged user

**man**: command manual

## Interacting w/ the File System

**ls**: listing files in current directory

**ls -a**: listing w/ hidden files

**cd**: change directory

**cat**: outputting contents of a file

**pwd:** print path to current working directory 

**touch**: create file

**mkdir**: create folder

**cp**: copy file/folder

**mv**: move file/folder

**rm**: remove file/folder

**file**: display file type

## Searching for Files

**find -name**: find a specific file by name

**grep**: search contents of files for specific values 

## Shell Operators

**&**: run commands in the background

**&&**: combine multiple commands in one line

**\>**: redirector w/ overwrite

**\>\>**: redirector w/ append 

## Secure Shell

**ssh**: log into remote machine using SSH

## Permissions

**su**: switch user

## Common Directories
+ **/etc**: system files
+ **/var**: variable data
+ **/root**: home directory for root user
+ **/tmp**: temporary files

## Terminal Text Editors

**nano**: terminal text editor

**VIM**: more advanced terminal text editor

## General/Useful Utilities

**wget**: download files via HTTP

**scp**: secure copy via SSH

**python3 -m http.server**: creates web server using local machine

## Processes

**ps**: list running processes by user

**ps aux**: list processes run by other users

**kill**: terminate process

Signals:

+ **SIGTERM**: terminate process after cleanup tasks

+ **SIGKILL**: terminate process w/o cleanup

+ **SIGSTOP**: stop/suspend process

**systemctl**: interact with systemd

Options:
+ **Start**
+ **Stop**
+ **Enable**
+ **Disable**

## Automation

<i>Crontab</i> -> a process that is started during boot that is responsible for facilitating and managing cron jobs

Requires 6 values:
+ MIN: what minute to execute at
+ Hour: what hour to execute at
+ DOM: what day of the month to execute at
+ MON: what month of the year to execute at
+ DOW: what day of the week to execute at
+ CMD: actual command to be executed
E.g. 0 */12 * * * cp -R /home/cmnatic/Documents /var/backups/

**crontab -e**: edit the crontab

## Package Management
**add-apt-repository**: automatically add a repository

Manually adding a repository:
1. **wget -qO - [software-gpg-download.gpg] | sudo apt-key add -**: download GPG key and use apt-key to trust it
2. Add to apt sources list (i.e. create a separate file for the repository)
3. **apt update**: recognise new entry
4. **apt install [software-name-here]**: install trusted software

Removing packages:
1. **add-apt-repository --remove ppa:[PPA_Name/ppa]**: remove apt file
2. **apt remove [software-name-here]**: remove installed software

## Logs
Logs can be located in /var/log directory.
