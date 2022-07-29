# How to setup make in Mac

* open /etc/bashrc
  
      sudo nano /etc/bashrc
 
 * enter the command at the end of the file and save with 
 
        complete -W "\`test -e Makefile && grep -oE '^[a-zA-Z0-9_-]+:([^=]|$)' Makefile | sed 's/[^a-zA-Z0-9_-]*$//'\`" make
