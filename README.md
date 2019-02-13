# termux-x
it is unofficial repository maintained by me @hax4us. you can check available packages in README

### List Of Available Packages (aarch64, arm)
1. xfce4 Desktop Environment (with all base dependencies)

#### How To Add My Repo
1. Add new sources list file `mkdir -p $PREFIX/etc/apt/sources.list.d && printf "deb https://hax4us.github.io/termux-x/ x11-stable main" > $PREFIX/etc/apt/sources.list.d/hax4us.list`
2. enable x11 repo `apt install x11-repo`
3. add public key `wget https://hax4us.github.io/termux-x/hax4us.key && apt-key add hax4us.key`
3. Update `apt update`

#### Inatall Any Package 
`apt install pkg_name`

#### Packages Will Be Add As Per Your Demand Guys :) (Just Open Issue As A Package Request)
