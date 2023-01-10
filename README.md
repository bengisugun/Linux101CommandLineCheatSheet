# Linux 101 Command Line Cheat Sheet


ls: List the files in a directory.

 
    $ ls
    file1.txt file2.txt dir1


cd: Change the current working directory.

    $ pwd
    /home/user
    $ cd dir1
    $ pwd
    /home/user/dir1


mkdir: Create a new directory.

 
    $ mkdir newdir
    $ ls
    file1.txt file2.txt dir1 newdir


touch: Create a new file.

 
    $ touch newfile.txt
    $ ls
    file1.txt file2.txt dir1 newdir newfile.txt


mv: Move or rename a file or directory.

 
    $ mv file1.txt dir1/
    $ ls dir1
    file1.txt
    $ mv file2.txt newfile2.txt
    $ ls
    dir1 newdir newfile2.txt


cp: Copy a file or directory.

 
    $ cp newfile.txt newfile_backup.txt
    $ ls
    dir1 newdir newfile2.txt newfile_backup.txt


rm: Remove (delete) a file or directory.

 
    $ rm newfile2.txt
    $ ls
    dir1 newdir newfile_backup.txt

rmdir: Remove (delete) an empty directory.

 
    $ rmdir newdir
    $ ls
    dir1 newfile_backup.txt


pwd: Print the current working directory.

 
    $ pwd
    /home/user

echo: Print a string of text to the console.

 
    $ echo "Hello, World!"
    Hello, World!

cat: Display the contents of a file.

 
    $ cat file1.txt
    This is the contents of file1.txt

less: View the contents of a file one page at a time.

 
    $ less file1.txt

head: Display the first few lines of a file.

 
    $ head -n 3 file1.txt


tail: Display the last few lines of a file.

 
    $ tail -n 3 file1.txt


grep: Search for a string of text in a file.

 
    $ grep "search_string" file1.txt


find: Search for files based on certain criteria.

 
    $ find . -name "file1*"


sort: Sort the lines of a text file.

 
    $ sort file1.txt > sorted_file1.txt


uniq: Display unique lines in a sorted file.

 
     $ uniq sorted_file1.txt


wc: Count the number of lines, words, and characters in a file.

 
    $ wc file1.txt


tar: Create or extract a tar archive file.

 
    $ tar -cvf archive.tar file1.txt file2.txt
    $ tar -xvf archive.tar


gzip: Compress or decompress a file using gzip.

 
    $ gzip file1.txt
    $ gunzip file1.txt.gz


zip: Compress or decompress a file using zip.

 
    $ zip archive.zip file1.txt file2.txt
    $ unzip archive.zip


chmod: Change the permissions of a file or directory.

 
    $ chmod 755 file1.txt


chown: Change the ownership of a file or directory.

 
    $ chown user:group file1.txt


df: Display free disk space on the file system.

 
    $ df -h


du: Display disk usage statistics for a file or directory.

 
    $ du -sh dir1/


ping: Send an ICMP echo request to a network host to check if it is reachable.

 
    $ ping google.com


traceroute: Trace the route that a packet takes to a network host.

 
    $ traceroute google.com


who: Display who is currently logged in.

 
    $ who


ps: Display the currently running processes.

 
    $ ps


kill: Send a signal to a process to terminate it.

 
    $ kill 1234


top: Display the currently running processes and their system resource usage in real-time.

 
    $ top


shutdown: Shut down or reboot a Linux system.

 
    $ sudo shutdown -h now


reboot: Shut down and restart a Linux system.

    $ sudo reboot
