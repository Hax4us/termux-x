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

#### Packages Will Be Add As Per Your Demand Guys :) (Just Open Issue As A Package Request)
