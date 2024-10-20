# Simple installation
```
sudo apt update
sudo apt install software-properties-common
sudo add-apt-repository --yes --update ppa:ansible/ansible
sudo apt install ansible
```

## Error 

```
"ERROR: Ansible requires the locale encoding to be UTF-8; Detected ISO8859-1"
```

### Fix :
```
step1
sudo nano /etc/default/locale

step2
LANG="en_US.UTF-8"
LC_CTYPE="en_US.UTF-8"

step3
sudo update-locale LANG=en_US.UTF-8 LC_CTYPE=en_US.UTF-8

step4
Finally restart your machine
```

