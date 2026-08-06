pwd
# Check current working directory / present working directory

whoami
# Check which user is currently logged in

date
# Display the current system date and time

date +%D
# Display date only in MM/DD/YY format

date +%T
# Display time only in HH:MM:SS format

date +%H:%M
# Display custom time format (Hours:Minutes)

ls
# List files and directories in the current folder

ls -lt
# List files sorted by last modified time in vertical format

ls -ltr
# List files in reverse sorted order (newest modified files at the bottom)

ls -lh
# List files with sizes displayed in human-readable format (K, M, G)

clear
# Clear the terminal screen (Shortcut: Ctrl + L)

cat file_name
# Display the complete contents of a file

less test.csv
# View file contents interactively with navigation and search capability

more test.csv
# View file contents page-by-page

touch new_file
# Create a new empty file

rm new_file
# Delete/remove a file

vi new_file
# Create or open a file in VI text editor

nano new_file
# Create or open a file in Nano text editor

mkdir new_folder
# Create a new directory/folder

rmdir new_folder
# Remove an empty directory/folder

rm -rf new_folder
# Forcefully remove a directory and all of its contents recursively

cd new_folder
# Change directory to enter a folder

cd ..
# Move back one directory level

cd ../..
# Move back two directory levels in one step

cd /
# Navigate directly to the root directory

cd ~
# Navigate directly to the logged-in user's home directory

cp mini.csv new_folder/
# Copy a file to a target directory

cp fileA.txt fileB.txt
# Copy contents of one file into another new file (duplicate/backup)

mv new_file new_folder/
# Move (cut and paste) a file to another folder

mv new_file new_file_modified
# Rename a file

head -5 test.csv
# Read/display the top 5 lines of a file

tail -5 test.csv
# Read/display the bottom 5 lines of a file

sort sort_demo.txt
# Sort file contents alphabetically (A to Z)

sort -r sort_demo.txt
# Sort file contents in reverse order (Z to A)

sort file.txt | uniq
# Display unique lines from a file by eliminating duplicates

split -l 3 file.txt
# Split a file into smaller files with 3 lines each

grep "corey" test.csv
# Search for a specific word/pattern inside a file

egrep "corey|anna" test.csv
# Search for multiple words/patterns simultaneously in a file

ls x*
# Use wildcard (*) to list all files starting with "x"

ls *.csv
# Use wildcard (*) to list all files ending with ".csv" extension

touch file{1..10}
# Use wildcards/brace expansion to create 10 files sequentially at once

shuf mini.csv
# Randomly shuffle the lines of a file

wc -l test.csv
# Count the total number of lines in a file

cmp fileA.txt fileB.txt
# Compare two files to check if they are identical

diff fileA.txt fileB.txt
# Compare and display line-by-line differences between two files

diff -u fileA.txt fileB.txt
# Unified diff output showing clear addition/deletion lines

find . -name test.csv
# Find a file by name starting from the current directory

find . -name "*.csv"
# Find all CSV files in current directory and subdirectories

locate test.csv
# Fast file search using the system database

sudo updatedb
# Update the locate database

history
# List previously executed commands in the terminal history

history | grep sort
# Search for specific commands previously executed in command history

ls --help
# Display syntax and available options/flags for a command

man ls
# Open the official user manual for a command

which ls
# Find the exact binary executable path of a command

bc
# Open the built-in basic terminal calculator

cal
# Display calendar for the current month

cal 2020
# Display full calendar for a specific year

cal Jan 2022
# Display calendar for a specific month and year

uptime
# Check server uptime, logged-in users, and system load average

script
# Record all terminal activity and output to a log file

exit
# Stop recording script / Exit current shell or user session

alias l="ls -ltr"
# Create a custom shortcut/alias for a long command

alias -p
# List all active system aliases

gzip -k test.csv
# Compress a file keeping the original file intact

gunzip test.csv.gz
# Decompress/unzip a gzip file

tar -czvf archive.tar.gz new_folder
# Compress an entire directory into a tar.gz archive

tar -xzvf archive.tar.gz
# Extract/decompress a tar.gz archive

zip myfiles.zip fileA.txt fileB.txt
# Compress multiple specific files into a single zip file

unzip myfiles.zip
# Unzip/extract a zip file archive

unzip -l myfiles.zip
# List contents of a zip file without extracting

wget https://www.python.org/ftp/python/3.11.1/Python-3.11.1.tgz
# Download files directly from a URL link

curl http://numbersapi.com/random
# Fetch data/responses or interact with web APIs from terminal

sudo yum install nginx
# Install a package/application using YUM package manager (RedHat/CentOS)

yum list installed
# List all installed packages on the system

yum list installed | grep java
# Check if a specific package (Java) is installed

dnf list available
# List all available packages ready for installation

systemctl status firewalld.service
# Check running status of a system service

sudo systemctl start nginx.service
# Start a system service

sudo systemctl stop nginx.service
# Stop a system service

systemctl list-units --type=service --all
# List all active and inactive system services

printenv
# Display all system environment variables

export JAVA_HOME=/usr/lib/jvm/java-17
# Set a temporary environment variable in shell

export PATH=$JAVA_HOME/bin:$PATH
# Update PATH variable with new binary path

source ~/.bashrc
# Apply changes made to environment variable files immediately

awk -F',' '{print $2}' test.csv
# Print a specific column (2nd column) from a CSV file

cut -c 1-2 mini.csv
# Display specific characters (1st to 2nd character) of each line

sed -n '5p' test.csv
# Print a specific line number (5th line) from a file

sed 's/business/finance/g' mini.csv
# Replace/substitute a specific word globally in output

tr 'a-z' 'A-Z' < test.txt
# Translate/convert lowercase letters to uppercase

tr -d '%' < test.txt
# Delete specific characters (%) from file content

truncate -s 50M fileA
# Extend or shrink a file size to a target size (e.g., 50MB)

echo "ABCDE" | fold -w 1
# Fold lines to wrap vertically at a specified width

su -
# Switch user to root / superuser

ssh user@10.21.55.5
# Remotely access a remote server over SSH

scp mac_file user@10.21.55.5:/home/user/
# Secure copy a file to a remote server over SSH

ls -la
# List all files including hidden files and permissions

chmod o+r sensitive_file
# Modify/add read permission for "other" users on a file

chown paul root_file
# Change owner of a file to a different user

chgrp paul root_file
# Change group owner of a file

free -h
# Check RAM memory usage in human-readable format

free -th
# Display total RAM and swap memory usage summary

top
# Real-time task manager to check CPU and RAM utilization per process

du -sh my_folder
# Check total disk space consumed by a specific folder

df -h
# Check disk space utilization across all mounted file systems

hostname
# Print current machine's network host name

lscpu
# Display detailed CPU cores, threads, and architecture information

arch
# Print system architecture type (e.g., x86_64)

lsblk
# List block storage devices and disk partitions

uname -a
# Print full system Linux kernel and OS information

cat /etc/os-release
# Print detailed Linux distribution distribution/version name

ps -ef
# List all active running processes

ps -ef | grep nginx
# Filter running processes for a specific service

pgrep nginx
# Get Process ID (PID) of a specific running application

sudo kill -9 8905
# Forcefully terminate/kill a running process using its PID

pkill httpd
# Terminate/kill running processes directly by application name

jobs
# List all active background/stopped jobs in current terminal

bg
# Resume a stopped job in the background

fg
# Bring a background job back to the foreground

nohup bash my_script.sh &
# Run a script continuously in the background detached from terminal

ifconfig
# Display network interfaces and server IP addresses

ping www.google.com
# Test network reachability and internet connectivity to a host

telnet 10.21.55.5 80
# Check if a specific IP address and port are open and reachable

netstat -tulnp | grep 80
# Check active listening ports and network connections

traceroute www.google.com
# Trace network route hops taken to reach a destination URL

useradd alex
# Create a new user account on the system

id alex
# Display user ID (UID) and group IDs (GID) for a user

passwd alex
# Set or change the password for a user account

groupadd testing
# Create a new user group

cat /etc/group
# Display group configuration file and created groups

userdel alex
# Delete a user account

groupdel testing
# Delete a user group

usermod -g testing nick
# Modify/change primary group of a user

at 05:10 PM
# Schedule a command to run once at a specific future time

ls -l > files.txt
# Redirect output of a command to a file (overwrites existing content)

echo "hostname" >> files.txt
# Append output of a command to the end of a file