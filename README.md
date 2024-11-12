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

wc -l t1.txt                                   : To print the line numbers of t1.txt

wc -w t1.txt                                   : To print word count of t1.txt

wc -c t1.txt                                   : To print tottal number of character in file t1.txt

echoo "hello"                                  : will display the given word

echo "good morning" > file1                    : will display the word in that file---> will overwrite 

echo "good day" >>file1                        : will display the currentt word and also the above word----> will nott overwrite

echo $?                                        : to chechk if my previous command has exicuted properly or not

head filename                                  : will display the first 10 lines in the file

tail filename                                  : will display bottom 10 lines

sort filename	                                 : To sort file in assending order based on the character

sort -n filename	                             : Sort file based on the numerical value

sort -r filename	                             : sort in reverse order

uniq	                                         : to show only uniq values (uniq will always used along with sort. without sort uniq will not work)

sort filename | uniq -c	                       : to display count of the values repeated

sort filename | uniq -d	                       : sort and display only duplicate values

sort -k1 -n filename                          : to sort the values based on the coulmn values

