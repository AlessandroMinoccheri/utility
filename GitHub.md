# GitHub

## Change or Set configuration account

```
 git config --global user.name "Alessandro Minoccheri"
 git config --global user.email alessandrominoccheri@gmail.com
```

Inside your repository you can add a configuration inside: .git/config
```
[user]
	name = Alessandro Minoccheri
	email = alessandro@studiomado.it
```

----

## Generate ssh keys for your project

```
ssh-keygen -t rsa -C "alessandrominoccheri@gmail.com"
cat ~/.ssh/id_rsa_whatyouwant.pub
```
