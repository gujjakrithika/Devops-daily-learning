Today's Learning:

Linux Basics and Command-Line Practice
1. Linux Fundamentals
Explored Linux and its importance in servers, cloud environments, containers, and DevOps.
Topics Covered:

Open-source software and Linux distributions (Ubuntu, Debian, RHEL).

Linux file system structure.

Package management.

Services and processes.

Containers and web servers.
2. Commands Practiced
File and Directory Management
pwd

ls

ls -la

cd

mkdir

cp

mv

rm

Practiced directory navigation and basic file operations.
System Information and Monitoring
free -h

df -h

top

uname -a

hostname

Learned to check memory, disk usage, running processes, and system information.
Package and Service Management
sudo apt update

sudo apt install nginx

systemctl status nginx

systemctl start nginx

systemctl enable nginx

Practiced installing Nginx and managing Linux services using APT and systemctl.
3. Working with grep
Focused on searching text within files, directories, and command outputs.
Commands Practiced:

grep -r copyright

grep -rl copyright

grep -R copyright

grep -r copyright | wc

grep -r copyright > lowercase.txt

grep -R copyright > uppercase.txt

diff lowercase.txt uppercase.txt

cat git/README.source | grep extracted

grep -A 2 extracted

grep -B 5 extracted

grep -C 4 extracted
Key Concepts Learned:

Recursive searching using -r and -R.

Displaying matching file names using -l.

Searching with context using -A, -B, and -C.

Output redirection using >.

Comparing files using diff.

Using pipes (|) to combine commands.
4. Process Management and Symbolic Links
ps aux

ps aux | grep root

ps aux | grep ^root

ps aux | grep d$

ls -l /usr/share/doc | grep debconf

Practiced monitoring and filtering running processes.

Explored basic pattern matching using ^ and $.

Understood symbolic links and how they reference existing files or directories.
5. Key Takeaways
Gained hands-on experience with essential Linux commands.

Understood basic system monitoring, package installation, and service management.

Improved understanding of grep, pipes, output redirection, and file comparison.

Explored process filtering, regular expressions, and symbolic links.

Learned practical command-line techniques useful for troubleshooting and DevOps workflows.
 
