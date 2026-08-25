How to download a file from internet ?
-> wget URL_OF_LIFE
wget -o opt_file.txt URL_OF_LIFE

How to call an api on linux ?
-> curl http://numbersapi.com/random

How to install an application on linux ?
-> apt or yum/dnf

How to check if an application is installed or not in linux ?
-> rpm -qa | grep app
dnf list installed

How to list available packages to install linux ?
-> apt search <package_name>
yum/def list available

How to start/stop a service on linux ?
-> systemctl start/stop service_name

How to list all sevices on linux ?
-> systemctl list-units --type = service --all

How to list all existing environment variables on linux ?
-> printenv

How to add a new environment varibles on linux ?
-> export JAVA_HOME = "/user/lib/jum/java_v" 
export PATH = $JAVA_HOME/bin:$PATH

How to add a new permenant environment variables in linux ?
-> add env variable in ./bashrc file source ~/.bash-profile

How to print a specific column from a csv file ?
-> awk -f, '{print $2}' file.csv

How to display starting two characters of all lines ?
-> cut -c1-2 file.txt

How to display a specific line from a file ?
-> sed -n 'sp' file.txt

How to replace a specific word in a file ?
-> set -n 's/from/to/g' file.txt

How to convert a content to uppercase or lowercase within a file ?
-> tr[:lower:][:upper:]<file.txt>
tr[:punch:]Z<file.txt>
tr[:digit:]Z<file.txt>

How to extend or shrink size of a file ?
-> truncate -s 100M file.txt

How to display following line in vertical line ? ABCDE
-> echo "ABCDE" | fold -w1

How to change user or login as different user in linux ?
-> su<user_name>

How to exit as current user or close terminal in linux ?
-> exit

If you are not root user, how to execute admin commands like installing new app ?
-> sudo yum install httpd