# Laravel / Homestead

Reference: https://laravel.com/docs/5.4/homestead

To working with laravel/homestead (a virtual machine already configurated for laravel) you need to download it:
```
vagrant box add laravel/homestead
```

This command add to your machine a new box with homestead

## Create a virtual machine with homestead
To create a virtual machine you need to crrate a directory, enter into it and use:
```
composer require laravel/homestead --dev
php vendor/bin/homestead make
vagrant up --provision
```

If you want to change some configuration you need to change these files:
```
Homestead.yaml
Vagrantfile
```

## Homestead for symfony
If you are working with symfony you need to change something inside your Homestead.yaml before launch vagrant up --provision like this:
Inside array"sites to" change public with web
After this line add this:
```
type: symfony
```

When you launch your symfony app with vagrant you can have this error:
```
You are not allowed to access this file. Check app_dev.php for more information.
```

To fix It you need to comment this line inside web/app_dev.php
```
exit('You are not allowed to access this file. Check '.basename(__FILE__).' for more information.');
```

## Hosts
Last thing you can do is to assign a name to your local app, you need to go into file: etc/hosts and add this line for example (ip and name depends on the parameters inserted into Homestead.yaml of your site)
```
192.168.10.10    your-site.app
```
