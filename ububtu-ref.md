# reset root user password
    sudo -i passwd

## switch user
    su <username>

## create user
    adduser <username>

## setup ssh for sudo user
- goto `cd ~` in <username>
- create `.ssh` folder using `mkdir .ssh/`
- create `authorized_keys` file inside the `.ssh` folder using `nano authorized_keys` 
- paste the public key of your shh keys into the file and save it
- you can now ssh into the user account with the private key of the public key


## adding a user to sudo group
#### reference [video on how to give a user sudo previlage](https://www.youtube.com/watch?v=WBgkuGQkwzk)
- switch to root user with `su root`
- goto file `/etc/sudoer`
- add the user to the line with `<username> ALL=(ALL:ALL) ALL`
- save and exit

## updating and upgrading ubuntu reference [upgrade and updte ubuntu](https://www.cyberciti.biz/faq/upgrade-update-ubuntu-using-terminal/)
- Open the terminal application
- For remote server use the ssh command to login (e.g. ssh user@server-name)
- Fetch update software list by running sudo apt-get update command
- Update Ubuntu software by running sudo apt-get upgrade command
- Reboot the Ubuntu box if required by running sudo reboot

## install pip for python 3
    sudo apt install python3-pip

## installing redis [blog to install redis](https://www.digitalocean.com/community/tutorials/how-to-install-and-secure-redis-on-ubuntu-18-04)


## display log from log file
    tail -f /path/to/log-file/log-file.log
