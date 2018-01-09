# Useful UNIX/DOS terminal commands

### how to find shell name

```bash
echo $0
```

### Verify the PID of current instance of shell

```bash
echo "$$"
```

### Verify the process having the PID

```bash
ps -p "$$"
```

### Verify the logname command prints the user-name of the current user

```bash
$ Logname
```

### Verify the uname command prints certain system information

```bash
$ uname -a
```

### Verify the passwd command is used for changing passwords for user accounts.

```bash
$ passwd manjeet
```

### Verify the grep command searches for a specified pattern in a file (or files) and displays in output lines containing that pattern.

```bash
$ grep Hello test.txt  
```

### Verify the id command prints user and group information for the current user or specified username.

```bash
$ id manjeet  
```

### Verify the pwd command displays the name of current/working directory.

```bash
$ pwd 
```

### The cd command is used to change the directory name

```bash
$ cd [directory-name] 
```

### Verify a specific port in DOS

```bash
netstat -ano | find /i "10060"
```

### Make all php files executable

```bash
chmod 777 `find . -name php -type d
```

### History of rm command on system

```bash
 find /home -name .bash_history -print | xargs grep -w rm
```

### Zip a directory

```bash
zip -r backup.zip /data
```

### Find all files in current directory

```bash
grep -H -r  "queue is in maintainence mode" .  
```

### TCP packet dump 

```bash
/usr/sbin/tcpdump dst 192.84.19.102 and port 5222 -X
```

### Who is listening on port 3000 

```bash
lsof -i :3000
```

### Grep all listening ports

```bash
lsof -i TCP | grep LISTEN
```

### Capture communication on UDP port

```bash
netstat -t -u -c | grep udp
```

### Check all listening port on machine

```bash
netstat -tpln
```

### Find and delete files

```bash
find . -name my_folder -exec rm -rf {} \;
```

### Compress folder

```bash
tar cfz myfile.tar.gz myfolder/
```

### Uncompress folder

```bash
tar xfz myfile.tar.gz
```

### Upload files

```bash
scp -P 1234 myfile.txt user@192.168.148.85:/some/folder
```

### Check free disk space

```bash
df -h
```

### Check size of directory contents

```bash
du -sh *
```

### Grep Java type usage

```bash
grep -or "com\.company\.project.\+" * | grep -o ":[a-zA-Z0-9\.]\+" | sort | uniq
```

### Pipe stdout and sterr to file

```bash
some_command > everything.txt 2>&1
```

### Java Thread Dumps

```bash
sudo jstack -F $PID > threads.log
```
### Copy data to vagrant vm

```bash
scp -P 2222 ../../neusns/neusns-build.zip vagrant@127.0.0.
```
### To change to root type on EC2 and to change root password

```bash
sudo -s  and then  sudo passwd
```
### To get processor architecture type (i386/i686 etc are32 bit)

```bash
uname -a and cat /proc/cpuinfo 
```
