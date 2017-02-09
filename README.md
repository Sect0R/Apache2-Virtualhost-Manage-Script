Apache2 Virtualhost Manage Script
===========

Bash Script to allow create or delete apache virtual hosts on Ubuntu on a quick way.

## Installation ##

1. Download the script
2. Apply permission to execute:

```
$ chmod +x /path/to/virtualhost.sh
```

3. Optional: if you want to use the script globally, then you need to copy the file to your /usr/local/bin directory, is better
if you copy it without the .sh extension:

```bash
$ sudo cp /path/to/virtualhost.sh /usr/local/bin/virtualhost
```

## Usage ##

Basic command line syntax:

```bash
$ sudo sh /path/to/virtualhost.sh [create | delete] [domain] [optional host_dir]
```

With script installed on /usr/local/bin

```bash
$ sudo virtualhost [create | delete] [domain] [optional host_dir]
```

### Examples ###

to create a new virtual host:

```bash
$ sudo virtualhost create mysite.dev
```
to create a new virtual host with custom directory name:

```bash
$ sudo virtualhost create anothersite.dev my_dir
```
to delete a virtual host

```bash
$ sudo virtualhost delete mysite.dev
```

to delete a virtual host with custom directory name:

```
$ sudo virtualhost delete anothersite.dev my_dir
```
