For Kali Linux:

| Commands             | Usage                                       |
| sudo apt-get update  | Pulls data from repositories and updates it |
| sudo apt-get install | Used to install packages on Kali            |

For github packages, it is simple to install. Find the package on GitHub, copy the link, _cd_ into /opt, and then run _git clone_ to get the package on your machine. Once that's done, the package should have instructions on how to actually install the tool/package.

You can combine commands with the && command.

ex: 
	apt update && apt upgrade
