# Dev-ops
uname            : To check OS

uame -r          : to check OS version

uname -m         : to check whether it is 32 bit or 64 bit

uname -a         : to check all details

uptime           : to know foor how longg the server is beiing running

who              : to check how many users are accessing the server at this moment

whoami           : to know the current logged users detailed

su "userrname"   : to switch the user

free             : to know how many disk space left 

free -m          : to know the above details in Mega bytes

free -g          : to know the details in Giga bytes

df -h            : this will let us know the used and free disk space

top              : to display all the running process and also lists its details

top -b n2        : this will make the top coommand to exit from the process after given time.

ps -eaf          : used to display the running process, but the process wont change or refresh and it will be fixed

date             : diplay the date

date +%Y-%M-%D   : display the date in year/month/date format

date +%Y-%m-%d   :to display in YYYY-MM-DD format

date +%Y-%m-%d -d "10 days ago" :to display date before 10 days

date +%Y-%m-%d -d "10 days" :to display date after 10 days

date +%Y-%m-%d" "%H:%M:%S :to display date and time in specified format

date +%Y-%m-%d" "%H:%M:%S -d "10 minutes ago" :to display time before 10 minutes

ps -eaf| grep firefox                          : this will  display the firefox process

ps -eaf | grep firefox | grep facebook         : will display the facebook process opened in firefox

kill "process id"                              : this will close the process 

kill -9 "process id"                           : forcefully close the process

pkill "process name"                           : to close the process or app

ls -ltr                                        : to list the directoory or the files which are in current path

ls -ltr filename                               : displayes if that file is  exists or not

pwd                                            : to know currently in whhich path you are in

cd "path"                                      : to switch to the next path---> change direcrtory

toouch filename                                : to create empty file

cat > filename                                 : to create a file with contents

cat filename                                   : to display the contents of the file

cat -n filename                                : willl display the contents and add arrange them in a number

tac filename                                   : display the file contents in reverse 
  
mkdir foldername                               : create a directory or folder

touch .filename or mkdir .filename             : will create a hidden file or directory

ls -latr                                       : to display the hidden file and directory

cp [source-file] [destination]                 : copy the file to the destination

cp [source-file] [var/source-file123]          : copies the source file to the var ddirectory with the different name

cp -r [directory1] [directory2]                : copies the contents with the folder

mv [file1] [file2]                             : moves the file1 to another destination with the rename

rm filename                                    : delete a file

rmdir -r directory                             : delete directory
