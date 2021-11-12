# setupEnvironment
In this repo i upload my setup instructions.....

# Linux OS
I Like to install any Linux Distribution (My Preference will be Ubuntu or Ubuntu based)

After Installation Run this following commands.
- For Update and Upgrade Your System :
    
      sudo apt update && sudo apt upgrade -y

- Then do a reboot(Not necessary But a good Practice) :
    
      reboot

- Then remove unnecessary Files by running this following command :

      sudo apt autoremove && sudo apt autoclean 

- Now I Always Like to Create a restore Point with timeshift :

      sudo apt install timeshift

- Now For fonts I Like to Install Windows Fonts :

      sudo cp -r Windows_Fonts/ /usr/share/fonts && sudo fc-cache -f

# Tools
- Browser :- 
    - Google Chrome
    - Firefox
    - Brave Browser
    - Edge
- Extensions :-
    - Ublock Origin
    - Privacy Badger
    - HTTPS Everywhere
- Text Editor :-
    - VIM
    - Sublime Text
    - Visual Studio Code

# Linux Applications and Tools
- gcc
- openjdk-17-jdk
- Python
- vim
- ncdu
- htop
- terminator 
- gnome-tweaks
- git

- For Installing all of this :

      sudo apt install openjdk-17-jdk vim ncdu htop brave-browser sublime-text terminator gnome-tweaks gcc git python3 -y

# Git Setup
- Step 1 :
    
      git config --global user.email ""
- Step 2 :
      
      git config --global user.name ""
- Step 3 :

      ssh-keygen -t ed25519 -C ""
- Step 4 :
    
      eval "$(ssh-agent -s)"
- Step 5 :

      ssh-add ~/.ssh/id_ed25519
- Step 6 :

      cat .ssh/id_ed25519.pub 

## VGA_Monitor.sh :-

Step 1 :- This to Check The Resolution Setting

    gtf 1920 1080 60

Step 2 :- This is For Adding New Mode using Xrandr

    xrandr --newmode "1920x1080_60.00"  172.80  1920 2040 2248 2576  1080 1081 1084 1118  -HSync +Vsync

Step 3 :- This For configure the Setting to your desktop environment
    
     xrandr --addmode VGA-1 "1920x1080_60.00"

Step 4 :- This is to Forcefully Generate the output
    
    xrandr --output VGA-1 --mode "1920x1080_60.00"