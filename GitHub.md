# GitHub

## Change or Set configuration account

```
 git config --global user.name "Alessandro Minoccheri"
 git config --global user.email alessandro.minoccheri@gmail.com
```

Inside your repository you can add a configuration inside: .git/config
```
[user]
	name = Alessandro Minoccheri
	email = alessandro.minoccheri@gmail.com
```

----

## Generate ssh keys for your project
I advise to leave empty the password for now

```
ssh-keygen -t rsa -C "alessandro.minoccheri@gmail.com"
```

To view your public key you can use:

```
cat ~/.ssh/id_rsa.pub
```

----

## How to push all your branches to master
Create a sh script like this inside root project

```
for remote in `git branch -r | grep -v master `; do git checkout --track $remote ; done
git push --all
```

And launch It from your console like this:

```
sh scriptname.sh
```
