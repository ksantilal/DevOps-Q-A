Linux
------------------------------------------
* Linux is an opensource operating system 

* How does the internet work?
- 
What is the server?
Difference between the web server and the application server?
* Types of applications?
* What are standalone apps?
* What are web applications?
* What are application support?
* What is application maintenance?


* What is linux?

### Navigation & Basics

* `/` -> represents root directory
* `pwd` -> present working directory
* `whoami` -> to check root user
* `mkdir` -> to craete a new folder or directory
* `mkdir -p devops/demo/demo2` -> if it's directory not available it will be create.
* `cd`-> change directory
* `cd ..` -> come back from the directory
* `ls`-> list of files and folders in the current directory
* `touch` -> to create a new file
* `echo` -> to print massege and also create a file by using this example:
`echo "hello world" > hello.txt`
* `cat` -> to read the content of a file
* `cp` -> to copy file example
`cp hello.txt hello_copy.txt` or `cp devops/1.txt cloud` <= copy from one folder to another
* mv -> to move file
`mv hello.txt hello_copy.txt` or `mv devops/1.txt cloud` <= copy from one folder to another
* `rm` -> to remove a file
`rm -r name of the folder`
* `rmdir` -> to remove a directory
# to run command as root user
`sudo su` => switch to super user

### Search & Filter

* `grep -i`  -> help to find word or anything which you want to find e.x. Awesome
* `grep -ir` -> it can scan evey single file and directory tp findout
* `find -name hello.txt` -> find anyfile or directory
* `awk` -> you can print column wise 
* `sed` -> to change strings or want amend the words

### Permissions

* `ssh-keygen` -> to create ssh key

* `chmod` -> to change the persmissons 
* `chown` -> change the ownership

### Monitoring

* `top` -> to check process
* `htop`
* `df -h` -> shows disc file system 
* `du -sh` -> disk utility
* `free -h` -> show you memory








* What is hardlink and softlink?
* links are sortcuts
* If your main file got deleted your softlink will deleted as well where as hardlink main file got deleted your hardlink will still available.
* ln -s path softlink
* ln path hardlinkfile
* What is process in linux?

