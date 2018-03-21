# Castle Init
> Initialization scripts for the Castle server

## Create New User
```bash
sudo adduser <newUser>
sudo visudo
```
Add the following:
```
<newUser> ALL = NOPASSWD: ALL
```
Log out, then back in as the new user.

## Delete Old User
```bash
sudo userdel -r pi
```

## Bootstrap
```bash
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install git
git clone https://github.com/mleone10/castle-init.git
cd castle-init
./install-packages
```

