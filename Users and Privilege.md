Example ls -la
{
total 88
	drwxr-xr-x  4 kalstorm kalstorm 4096 Dec 29 14:42 .
	drwxr-xr-x 10 kalstorm kalstorm 4096 Dec 28 15:15 ..
	-rw-r--r--  1 kalstorm kalstorm  824 Aug  2 22:48 Common Ports and Protocols.md
	-rw-r--r--  1 kalstorm kalstorm    0 Jul 29 21:38 CyberSec.md
	drwxr-xr-x  2 kalstorm kalstorm 4096 Aug  1 23:07 diary
	drwxr-xr-x  8 kalstorm kalstorm 4096 Aug  3 00:04 .git
	-rw-r--r--  1 kalstorm kalstorm 4549 Dec 22 14:06 HTML.md
	-rw-r--r--  1 kalstorm kalstorm  120 Dec 28 18:25 index.md
	-rw-r--r--  1 kalstorm kalstorm  694 Aug  1 23:58 IP Addresses.md
	-rw-r--r--  1 kalstorm kalstorm  138 Dec 29 14:22 Kali.md
	-rw-r--r--  1 kalstorm kalstorm  104 Dec 29 14:42 Linux.md
	-rw-r--r--  1 kalstorm kalstorm  391 Aug  2 00:04 MAC Addresses.md
	-rw-r--r--  1 kalstorm kalstorm  961 Dec 29 14:41 Navigating the Filesystem.md
	-rw-r--r--  1 kalstorm kalstorm  229 Dec 28 18:24 Networking.md
	-rw-r--r--  1 kalstorm kalstorm   81 Dec 28 18:24 Notes Directory.md
	-rw-r--r--  1 kalstorm kalstorm  543 Aug  2 22:57 OSI Model.md
	-rw-r--r--  1 kalstorm kalstorm   42 Dec 28 18:25 Practical Ethical Hacking.md
	-rw-r--r--  1 kalstorm kalstorm  188 Dec 21 00:34 Programming Languages.md
	-rw-r--r--  1 kalstorm kalstorm    0 Jul 29 22:00 README.md
	-rw-r--r--  1 kalstorm kalstorm 2418 Aug  3 00:03 Subnetting.md
	-rw-r--r--  1 kalstorm kalstorm  323 Dec 29 14:31 Sudo.md
	-rw-r--r--  1 kalstorm kalstorm  471 Aug  2 00:15 TCP-UDP-Three-Way Handshake.md
	-rw-r--r--  1 kalstorm kalstorm   15 Dec 29 14:42 Users and Privilege.md
}
r = read, w = write, x = execute

Each listing has a first column, and then 3 groups of 3 letters. The first group is the owner of the file. The second set of 3 is permissions for members of the group that owns the file. The last grouping is the permissions for all other users.

_chmod_ stands for change mode. + adds privileges, - takes away privileges. You can also use numbers with _chmod_ to specify all privileges. 777 = Full r,w,x privileges for all users

_adduser_ creates a new user. These users can be seen in the /etc/passwd file. The passwords are stored in the /etc/shadow file.

New users don't have access to _sudo_, and are not initially in the sudoers file.
