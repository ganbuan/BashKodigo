# BashKodigo
Cheat sheet for common Bash commands 

**echo**: Output any provided text

**whoami**: Display current logged user

**man**: command manual

**ls**: listing

**ls -a**: listing w/ hidden files

**cd**: change directory

**cat**: concatenate

**pwd:** print working directory 

**find -name**: find a specific file by name

**grep**: search contents of files for specific values 

**&**: run commands in the background

**&&**: combine multiple commands in one line

**\>**: redirector w/ overwrite

**\>\>**: redirector w/ append 

**ssh**: log into remote machine using SSH

**touch**: create file

**mkdir**: create folder

**cp**: copy file/folder

**mv**: move file/folder

**rm**: remove file/folder

**file**: display file type

**su**: switch user

Common directories:
+ **/etc**: system files
+ **/var**: variable data
+ **/root**: home directory for root user
+ **/tmp**: temporary files

**nano**: terminal text editor

**VIM**: more advanced terminal text editor

**wget**: download files via HTTP

**scp**: secure copy via SSH

**python3 -m http.server**: creates web server using local machine

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

**add-apt-repository**: automatically add a repository

Manually adding a repository:
1. **wget -qO - [software-gpg-download.gpg] | sudo apt-key add -**: download GPG key and use apt-key to trust it
2. Add to apt sources list (i.e. create a separate file for the repository)
3. **apt update**: recognise new entry
4. **apt install [software-name-here]**: install trusted software

Removing packages:
1. **add-apt-repository --remove ppa:[PPA_Name/ppa]**: remove apt file
2. **apt remove [software-name-here]**: remove installed software

