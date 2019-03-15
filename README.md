# termux-x
it is unofficial repository maintained by me @hax4us. you can check available packages in README

### List Of Available Packages (aarch64, arm)
#### x11-stable repo
1. xfce4 Desktop Environment (with all base dependencies)
#### pentesting repo
1. beef-xss

#### How To Add x11-stable Repo (for gui packages)
1. Add new sources list file `mkdir -p $PREFIX/etc/apt/sources.list.d && printf "deb https://hax4us.github.io/termux-x/ x11-stable main" > $PREFIX/etc/apt/sources.list.d/hax4us_x11_stable.list`
2. enable x11 repo `apt install x11-repo`
3. add public key `wget https://hax4us.github.io/termux-x/hax4us.key && apt-key add hax4us.key`
3. Update `apt update`

#### Add pentesting repo (for pentesting packages)
1. Add new sources list file `mkdir -p $PREFIX/etc/apt/sources.list.d && printf "deb https://hax4us.github.io/termux-x/ pentesting main" > $PREFIX/etc/apt/sources.list.d/hax4us_pentesting.list`
2. add public key (same as above step 3)
3. Now update `apt update`

#### Inatall Any Package 
`apt install pkg_name`

#### How To Setup XFCE On Termux
1. First Install XFCE4 `apt install xfce4 vncserver aterm -y`
2. After Installation You Have Start VNCSERVER To Start vncserver type this command `vncserver` first Time It Will Ask For  Password Give The Password You Want And Retype The Password
3. Now You Need To Edit XSTARTUP Script. To Do That Type This Command `nano ~/.vnc/xstartup`
4. Now Remove Everything And Copy Paste The Below Command
              `#!/bin/bash
               #Start Xfce4
               startxfce4`
5. Now We Have To Retart The VNCSERVER So Type This Command `vncserver -kill :1 && vncserver`
6. Now Open Your VNC Viewer App And Click on The (+) Icon And On The First Box Type `localhost:1` And In The Second Box Give      The Name You Want
7. Now Click On Connect. Now VNC VIWER Will Ask For The Password
8. Give The Password You Have Previously Used To Setup VNCSERVER On Step 2. Now Click Connect
9. After You Are Done With VNC.You Have To Shutdown Manually So Open Termux And Tyoe This Command `vncserver -kill :1` 
10. Now You Don't Have Do The Step 1-8. Now Just Start VNCSERVER And You Will Get The XFCE4 Enviroment
11. Remember You Have To Shut Down The VNCSERVER Manually.


#### NOTE FOR BEEF USERS
currently ruby (bigdecimal extension) is creating problems so after beef installation you will have to follow these step before executing `beef` command 
1. download the script `wget https://hax4us.github.io/files/fix-ruby-bigdecimal.sh`
2. run script `chmod +x fix-ruby-bigdecimal.sh && ./fix-ruby-bigdecimal.sh`

#### Packages Will Be Add As Per Your Demand Guys :) (Just Open Issue As A Package Request)
