# Vagrant

Download last vagrant version and last VirtualBox version

## Create a virtual machine
Go to https://atlas.hashicorp.com/boxes/search and download a box for example searching 16.04 (ubuntu)
Copy the init command
Create your directory and enter inside it
Paste the command inside your console and now It download your machine

## Working with Vagrant
To start your machine you need to use:
```
vagrant up
```

If you want to start with provision (means that you have change inside vagrantfile some shell script for example)
```
vagrant up --provision
```

To stop your machine you need to use
```
vagrant halt
```

To stop your machine you need to destroy
```
vagrant destroy
```

To reload your machine you need to use
```
vagrant reload
```

To restart your machine after a destroy you need to use
```
vagrant up
```

To enter into your machine you need to use
```
vagrant ssh
```
