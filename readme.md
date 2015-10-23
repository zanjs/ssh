### ssh
Administrator@WIN-9PH4ISN44NM MINGW64 /e/zan/www/gitpages
$ cd ~/.ssh

Administrator@WIN-9PH4ISN44NM MINGW64 ~/.ssh
$ ls
github_rsa  github_rsa.pub  id_rsa  id_rsa.pub  known_hosts

Administrator@WIN-9PH4ISN44NM MINGW64 ~/.ssh
$ rm *

Administrator@WIN-9PH4ISN44NM MINGW64 ~/.ssh
$ ls

Administrator@WIN-9PH4ISN44NM MINGW64 ~/.ssh
$ cd ~

Administrator@WIN-9PH4ISN44NM MINGW64 ~
$ ssh-keygen -t rsa -C "root@zanjs.com"
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/Administrator/.ssh/id_rsa):
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/Administrator/.ssh/id_rsa.
Your public key has been saved in /c/Users/Administrator/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:gAYTmJ1YHu4Sl+O+7gRm/kquVfseC8cz2WRNA9tCQfM root@zanjs.com
The key's randomart image is:
+---[RSA 2048]----+
| **o   .*.       |
|+oo= . . *       |
|. * o . o E      |
| = o   . + .     |
|ooo .   S .      |
|++ . o =         |
| o+ o B .        |
|oo.. + =         |
|o==. .+          |
+----[SHA256]-----+

Administrator@WIN-9PH4ISN44NM MINGW64 ~/.ssh
$ git config --global user.name "zanjs"

Administrator@WIN-9PH4ISN44NM MINGW64 ~/.ssh
$ git config --global user.email "root@zanjs.com"

$ ssh -T git@github.com
The authenticity of host 'github.com (192.30.252.131)' can't be established.
RSA key fingerprint is SHA256:nThbg6kXUpJWGl7E1IGOCspRomTxdCARLviKw6E5SY8.
Are you sure you want to continue connecting (yes/no)? yes
Warning: Permanently added 'github.com,192.30.252.131' (RSA) to the list of known hosts.
Enter passphrase for key '/c/Users/Administrator/.ssh/id_rsa':
Hi zanjs! You've successfully authenticated, but GitHub does not provide shell access.
