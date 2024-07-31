# aquarium-CLI
```
     |\    o
    |  \    o
|\ /    .\ o
| |       (
|/ \     /
    |  /
     |/
```
#### Follow these steps one by one: 
- Clone this repository in `/tmp` folder on your linux machine 
- 1st Step is to install library libcurses-perl
```bash
sudo apt-get install libcurses-perl
cd /tmp/aquarium-CLI
git clone https://github.com/0xT3sla/aquarium-CLI.git
tar -zxvf Term-Animation-2.4.tar.gz
cd Term-Animation-2.4/
perl Makefile.PL && make && make test
sudo make install
```
- 2nd step is to install the aquarium
```bash
cd /tmp/aquarium-CLI
tar -zxvf asciiquarium.tar.gz
cd asciiquarium_1.1/
sudo cp asciiquarium /usr/local/bin
sudo chmod 0755 /usr/local/bin/asciiquarium
```
- 3rd to run it, 
```bash 
perl /usr/local/bin/asciiquarium
```
- 4th step , to make this as linux command
```bash
cd ~
nano .bashrc
```
- Enter this at the end of all the contents in `.bashrc`
```bash
alias fish-tank='perl /usr/local/bin/asciiquarium'
```
- Press ctrl + x , then save it by saving 'Y' and press enter to confirm the name.

final step: use the command `fish-tank` to run the aquairum and to quit it press Q.

*only do this if you have an idea about bashrc editing don't mess it up ;)

Enjoy the aquarium when your home laptop/server sits idle. 🐟🐠🎣

---
source: [https://youtu.be/6euagWeOVck?feature=shared](https://youtu.be/6euagWeOVck?feature=shared)
