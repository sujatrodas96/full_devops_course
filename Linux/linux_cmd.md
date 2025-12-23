======================== LINUX COMMANDS WITH PURPOSE (DEVOPS 2+ YEARS) ========================

-------------------- BASIC LINUX COMMANDS --------------------

1. pwd -- To show current working directory
2. ls -- To list files and directories
3. ls -l -- To list with detailed info
4. ls -a -- To show hidden files
5. ls -lh -- To show human-readable sizes

6. cd <dir> -- To change directory
7. cd .. -- To move one step back
8. cd / -- To go to root directory
9. cd ~ -- To go to home directory

10. mkdir <name> -- To create directory
11. mkdir -p a/b/c -- To create nested directories

12. touch <file> -- To create empty file
13. rm <file> -- To remove file
14. rm -r <dir> -- To remove directory
15. rm -rf <dir> -- To force delete directory (dangerous)

16. cp source dest -- To copy file
17. cp -r source dest -- To copy folder
18. mv source dest -- To move or rename

19. cat <file> -- To view file content
20. tac <file> -- To view file in reverse
21. nl <file> -- To show line numbers
22. head <file> -- To show first 10 lines
23. tail <file> -- To show last 10 lines
24. tail -f <file> -- To monitor logs live

25. file <filename> -- To check file type
26. which <command> -- To show command executable path
27. whereis <cmd> -- To locate binary, source & man page

-------------------- PERMISSIONS & OWNERSHIP --------------------

28. chmod 777 <file> -- Full permission
29. chmod 755 <file> -- Read & execute for all
30. chmod 644 <file> -- Read write owner only
31. chown user <file> -- Change owner
32. chown user:group <file> -- Change owner & group
33. chgrp group <file> -- Change group

-------------------- SEARCHING & FINDING --------------------

34. find /path -name filename -- To find file by name
35. find / -type f -- To find files only
36. find / -type d -- To find directories only
37. grep "text" file -- To search text
38. grep -i "text" file -- Case insensitive search
39. grep -r "text" dir -- Recursive search in directory
40. grep -n "text" file -- Show line numbers
41. egrep "a|b" file -- Search multiple patterns

-------------------- ARCHIVE & COMPRESS --------------------

42. tar -cvf file.tar dir -- Create tar
43. tar -xvf file.tar -- Extract tar
44. tar -czvf file.tar.gz dir -- Create tar gzip
45. tar -xzvf file.tar.gz -- Extract gzip

46. zip file.zip file -- Create zip
47. unzip file.zip -- Extract zip

-------------------- SYSTEM INFO & RESOURCES --------------------

48. uname -a -- Show system info
49. hostname -- Show system hostname
50. hostnamectl -- Show OS + kernel details

51. date -- Show current date/time
52. cal -- Show calendar

53. df -h -- Show disk usage
54. du -sh -- Show folder size
55. du -sh * -- Show size of everything in folder

56. free -h -- Show memory usage
57. top -- Show running processes
58. htop -- Advanced process viewer
59. ps aux -- Show all running processes
60. kill <PID> -- Kill process
61. kill -9 <PID> -- Force kill process

-------------------- USER MANAGEMENT --------------------

62. whoami -- Show current user
63. who -- Show logged in users
64. id -- Show user info
65. sudo su -- Switch to root
66. su - user -- Switch user

67. useradd <name> -- Create new user
68. passwd <user> -- Set user password
69. userdel <user> -- Delete user
70. groupadd <group> -- Create group
71. usermod -aG group user -- Add user to group

-------------------- FILE VIEW & EDIT --------------------

72. vi <file> -- Open file in VI editor
73. vim <file> -- Open in vim
74. nano <file> -- Open in nano editor

VI SHORTCUTS
75. i -- Insert mode
76. Esc -- Exit insert mode
77. :w -- Save
78. :q -- Quit
79. :wq -- Save & quit
80. :q! -- Quit without save

-------------------- DOWNLOAD & TRANSFER --------------------

81. wget <url> -- Download file
82. curl <url> -- Fetch URL data
83. scp file user@host:/path -- Secure copy to remote
84. scp user@host:/file . -- Copy from remote

-------------------- PACKAGE MANAGEMENT --------------------

APT (Ubuntu / Debian)
85. apt update -- Refresh repo
86. apt upgrade -- Upgrade packages
87. apt install pkg -- Install package
88. apt remove pkg -- Remove package
89. apt purge pkg -- Remove including config

YUM / DNF (RHEL / CentOS)
90. yum install pkg -- Install
91. yum update -- Update
92. yum remove pkg -- Remove

-------------------- SHELL & SCRIPTING COMMANDS --------------------

93. sh script.sh -- Run shell script
94. bash script.sh -- Run bash script
95. chmod +x script.sh -- Make script executable
96. ./script.sh -- Execute script

VARIABLES
97. VAR=value -- Set variable
98. echo $VAR -- Print variable
99. export VAR=value -- Export variable

LOOPS
100. for i in 1 2 3; do echo $i; done -- For loop
101. while true; do echo hi; done -- While loop

-------------------- NETWORKING COMMANDS (VERY IMPORTANT) --------------------

102. ifconfig -- Show IP details (older)
103. ip addr show -- Show IP (modern)
104. ip link show -- Show NIC details

105. hostname -I -- Show IP only
106. ping <host> -- Check connectivity
107. ping -c 4 <host> -- Ping 4 times only

108. curl ifconfig.me -- Show public IP
109. nslookup domain -- DNS lookup
110. dig domain -- Detailed DNS lookup

111. traceroute host -- Show packet path
112. tracepath host -- Alternative traceroute

113. netstat -tulnp -- Show listening ports (older)
114. ss -tulnp -- Show listening ports (modern)

115. telnet host port -- Check port connectivity
116. nc -zv host port -- Check port open/closed

117. route -n -- Show routing table
118. ip route show -- Show route (modern)

119. arp -a -- Show ARP cache

-------------------- FIREWALL (BASIC) --------------------

120. ufw status -- Show firewall status
121. ufw enable -- Enable firewall
122. ufw allow 22 -- Allow SSH
123. ufw deny 80 -- Block port 80
124. ufw disable -- Disable firewall

-------------------- LOGS --------------------

125. /var/log/syslog -- System logs
126. /var/log/auth.log -- Authentication logs
127. journalctl -- View systemd logs
128. journalctl -xe -- View detailed logs
129. dmesg -- Kernel logs

-------------------- CRON JOBS --------------------

130. crontab -e -- Edit cron jobs
131. crontab -l -- List cron jobs

CRON FORMAT
minute hour day month weekday command

Example:
*/5 * * * * script.sh -- Run every 5 min

-------------------- SERVICES (SYSTEMCTL) --------------------

132. systemctl status service -- Check service status
133. systemctl start service -- Start service
134. systemctl stop service -- Stop service
135. systemctl restart service -- Restart service
136. systemctl enable service -- Enable on boot
137. systemctl disable service -- Disable boot

-------------------- DISK & MOUNTING --------------------

138. lsblk -- Show disk and partitions
139. fdisk -l -- Show disk info
140. mount /dev/sdX /mnt -- Mount disk
141. umount /mnt -- Unmount disk

-------------------- IMPORTANT FOR DEVOPS INTERVIEWS --------------------

✔ Linux commands + logs
✔ Shell scripting basics
✔ Process management
✔ Disk, CPU, Memory monitoring
✔ Networking + ports
✔ Cron jobs
✔ Services handling
✔ Permissions & users

================================================================================
