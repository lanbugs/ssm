# ssm - SSH Shell Menu
SSH Shell Menu written in Python

![example](https://lanbugs.de/wp-content/uploads/ssm.png)

This is a small python script for a shell menu to manage ssh connections.

# Requirements
* python3
* dialog
* pythondialog 

# Installation

## Install Debian packages and pip packages

```
apt install python3 python3-pip python3-setuptools dialog
pip3 install -r requirements.txt
```

## Copy ssm to /usr/bin/local

```
cp ssm /usr/bin/local
chmod +x /usr/bin/local/ssm
```

## Create connections.ini

Create folder in home directory and create connections.ini file.

```
mkdir ~/.ssm
touch connections.ini
```

For each server create a new section in the connections.ini file.

```
[example1]
description=Example1 Server
user=root
server=server1.example.org
port=22
options=
ssh_key=
```

# Use it!

```
ssm
```
