# Linux commands
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

 head 				                               	- displays first 10 lines from the file.

53.  head -5 filename			                  	- first 5

54:  tail		                            			- last 10 and enter -4 to show just last 4

55:   uptime 	                        				- to check the load avg

56:  cat  /proc/cpuinfo       	          		- shows how many core processor configured in server

57:  ps 					                            -running process

58:  dmidecode			                      		- hardware details of the server

59:  dmidecode -t bios 		                		- to display it

60:  vim filename			                      	- edit a file

70:  More filename 				                    - use enter and space for the scroll.

80:  runlevel				                        	- who -r   . 0-6 runlevel and 3 for cmd line and 5 for graphical mode and so on

81:  useradd <username>	                			- create a user. 3 types of users-- root, system, and normal.

82:  cat /etc/passwd	                  			- to check the users list.

83:  getent passwd username		              	- to check the ids

84:  cat /etc/shadow			                  	- to know if the password has been set to the users.

85:  passwd -d username			                	- delete the password of the user

86:  passwd username			                  	- reset the password 

87:  usermod -u userid username		          	- change the user id of the user

88: groupmod -g groupid username		          - change the group id

89: usermod -c <caption> <username>	        	- add captions for the existing usr

90: usermod -d <new home directory path> usrname- to change the home directory of the user- no 83 is to check the home directory.

91:  cat /etc/shells				                - to check all the shells

92:  usermod -s <shell> username	        	- change the shell. or chsh username to change it

93: ps -p $$			                      		- check the current shell.
you can also use, getent passwd username to check the shell.



94: usermod -u<userid> -c<caption> -s<shell>usr - to set this while creating user

95: .bash_profile			                      	- first file to open. and it is a direct login. vim .bashprofile and we can enter any cmd and while logging in directly, the entered cmd's will also execute.

96: .bashrc				                          	- works both in direct and indirect login.

97: echo $PATH			                      		- shows all the path where the user has access to.

98: which uptime		                      		- it will show its path. and using echo $PATH and remove the uptime's path, theh uptime cmd wont execute. and this will only work on current session.

99: export PATH=$PATH:/usr/bin		          	- to add the deleted cmd from the echo $PATH

100: To remove the cmd permentely, login to .bash profile and remove that path.

101: .bash_history			                    	- contains all the cmd's executed by the user.

102.  bash_logout				                      - executes when we exits the current session

103. groupadd groupname		                		- used to create a group.

104. cat /etc/group		                    		- check the groups list.

105: usermod -G grpname usrname		          	- add the user to group 

106: groupadd groupname		                		- create a group.

107: usermod -G grpname username	          	- add the user to the group

108: groups username				                  - to see the user is part of which group.

109: getent group <grp name>		            	- to see which all users are in that grp.

110: usermod -a -G groupname username	      	- to add the user to another group without removing from the current grp.

111: passwd -d username			                	- deletes the passwords for the user

112: gpasswd -d username grpname	          	- remove the user from the grp.

113: groupdel grpname	                  			- remove group

114: usermod -g grpname username		          - add the user to the primary grp.

115: passwd -l username			                 	- lock the password-- can check if the user has the password lock in /etc/shadow

116: passwd -u username			              	- unlock the pass lock

117: chage -l username			              	- to know the age of the user

118: chage -E "2022-12-20" username	      	- set the expiration date for the password

119: chage -d 2022-12-27 username 	      	- set the acc passwd expiry

120: chage -W 10 username			              - passwd expiry warning in days

121: getent passwd username			            - to check the shell applied to the user as a root user

122: cat /etc/ssh/sshd_config			          - to check the login or modify it 

123: chown username file name			          - to make the user as its owner.

chown -R username foldername		          	- to make the user owner of all the subdirectories

124: chmod *** filename			              	- to give the permission.

125: and once you give the permission to the group, you need to use the cmd as chgrp groupname filename -- it is used to make that group as part of that file so that the permission is applied


126: chmod *** directory name			- give permission to the group

127: chmod -R *** direcotory name		- permission is applied to all the subfolders.


128: chgrp -R groupname directory name		- so that the group is added to that directory and its subs

129: du -sh					- to know the size of the file. stat filename, du -h file name will also work.

130: chmod o+t directory name 			- give the full permission for the user via permission cmd, but sticky cmd wont be able delete the directory. o-t is to remove. [sticky bit]

140: chgrp -R groupname folder name		- this will make the folder and files created to be under that group.

141: chmod g+s foldername 			- will affect the above cmd to the future created files too.

142: setfacl -R -m u:username: rwx folderpath	- it is giving access to only one particular user.

142: getfacl directory name			- to check the details of the abve cmd given. if we give ls -ltr  if there is + then the setfacl is active.

143: setfack=l -x u:username filename  		- to remove the facl

144: setfacl -R -m g:groupname: rwx folderpath  - to set to groups.

145: setfacl -b filenamwe			- removes all the acl

146: paswd -s username				- to check if the password is locked.

147: single usermode    			- to change the password of the root user

148: usermod -d current path username		- tos change the home directory of the user, you  check the home directory by using getent passwd username.

149: usermod -s /sbin/nologin username		- this is the shell where the user wont be able to login.

150: getent group groupname			- to know the users in that groups.

151: gpasswod -d username group			- remove the user from the group

152:chmod u+s filepath (usr/bin/passwd)		- this will be used so tht the user will be able to perform this task, like changing his own password.

153: umask ***					- if the user creates an file, the permission should be same as we set. 666 is the max permissomn for the file and we want to set 646. So it would be 666-646 which is 020. So the cmd is umask 020  And this is only for this session and to make it permanent, you have to add it to the bash profile.

154: umask -S 					- to know the current umask value.

155: zip destination> <source>			- this will zip the file.

156: gzip file					- directly zip the file with no copy created.

157: unzip -l zip file				- to know the source file of the zip

158: gunzip -l zip file				- to know the source file of the gzip method.

159: gunzip zipfile (gzip method)		- used to unzip the gz zip file.

160: unzip zip file				- used to unzip the file.

161: tar -cvf destination dir> <source dir	- used to compress the directory, but first we need to convert it into tar.

162: gzip dir.tar				- then convert that into zip.

163: gunzip dir.gz				- to unzip it

164: tar -tvf dir.tar				- to see the contents of the tar folder.

165: tar -xvf dir.tar				- to extract the tar file.

166: stat or ls -li 				- to know the inode number of the file.

167: df -i 					- to check the inode partition details 

168: ln sourcefile newfile1=			- create hard link- changes made in one file will also show up in another.(can only be applied to files) -- EVEN if the source is deleted, the hard link will be accessible.
	
169: lane -s source destination			- create the soft link.
can be used for both directory and files. diff inode number

170: unlink newfile				- unlink the soft and hard link

171: SSH -- used to connect the server remotely

/etc/ssh/sshd_config
port number is 22
service sshd

172: vim /etc/ssh/sshd_config			- edit and enter AllowUser username and then save it. >>> service sshd restart
>> now only the added user can be able to login and other gets an access denied error.
 to add the group, you have to add AllowGroups groupname

173: Do the same as DenyUser username		- this is restrict that particular user.	

174: vim -f /etc/sudoers			- edit and enter this.
username ALL=(ALL)/path  this will grant the access to that user to perform that cmd.
and if we want that user not to perform one particular cmd, then use username ALL=(ALL) ALL, ! that path

175: sudo -l 					-to know the user access of the sudo access 

176: username ALL=(ALL) NOPASSWD: ALL		- this will prevent the server from asking the password for the sudo user.

177: %group name ALL=(ALL) path			- this is for the group access.

179: reason for not able to login-- 
1: it should not be /sbin/nologin
2: check secure logs whether the user entered the wrong pass
3: chage -l username	- to know the expiry
4: check in etc/ssh/sshd_config

178: service status crond			- to check its status
 service --status-all    to check all the services status

179: find . -type f -user root
 
180: grep "content" path			- used to search the content in he path. you can also use grep -o "content" path -l -c -v etc.

181: find path -type action 

182: stat filename/dir name  			- to check the full details of the file also the inode.

183: ls -li file				- to check the inode

184: df -h					- to check the partition details with storage.

185: df -i					- to check the inode partition.

186: netstat -a 				- shows all port number

187: netstat -tlnp 				- number of tcp

