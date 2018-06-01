# Minimal LAMP Stack
Minimal LAMP Stack provide Ubuntu 18.04, Apache, PHP7.1, MySQL, phpMyAdmin in a flexible box for Vagrant.

## Prerequisites

Be sure to install [VirtualBox](https://www.virtualbox.org/wiki/Downloads), [Vagrant](https://www.vagrantup.com/downloads.html) and optionally [Git](https://git-scm.com/downloads).

## First time initialization:

#### From command line
```
$ git clone https://github.com/LeonardoPuccio/Minimal-LAMP-Stack my-workspace
```

#### GUI
Simply [download](https://github.com/LeonardoPuccio/Minimal-LAMP-Stack/archive/master.zip) and extract Minimal-LAMP-Stack-master.zip where do you want.

## How to use

#### Start
```
$ vagrant up
```

#### Stop
```
$ vagrant halt
```
#### Accesses

##### - From browser go to
> [http://192.168.33.10/](http://192.168.33.10/)
or
> [http://localhost/](http://localhost/)  

to see [phpinfo()](http://php.net/manual/en/function.phpinfo.php).

##### - phpMyAdmin
>[http://192.168.33.10/phpmyadmin/](http://192.168.33.10/phpmyadmin/)
or [http://localhost/phpmyadmin/](http://localhost/phpmyadmin/)

##### - Shared folder
The `www` folder is a shared folder synced with `/var/www/html` in ubuntu virtual machine that correspond to default root folder of the web server.

*Is possible access to database from a desktop client such as Sequel Pro or HeidiSQL.
Remind you need ssh tunneling.*

## In the box
- Ubuntu-18.04 (live-server-amd64)
- Apache (2.4.29)
- PHP7.1 (7.1.17)
- MySQL (5.7.22-0)
- phpMyAdmin

## Default Credential:  

#### - Ubuntu Root Login
> root: vagrant  
> password: vagrant  

#### - DataBase Users

##### &nbsp; &nbsp;MySQL Admin* for phpMyAdmin  
> user: vagrantdb  
> password: vagrantdb

##### &nbsp; &nbsp;MySQL Root
> user: root  
> password: root

*Note: vagrantdb is an user with all privileges on vagrantdb, this for avoid conflict problem with phpmyadmin and access to it.*
