# Inside Docker

1. Install Git 2
2. Install Python(conda)
3. Install nvm 
4. Install node


### Install git from IUS

```
sudo yum -y install  git224-all.noarch 
```

```
sudo yum list | grrep -i git
```
#####

#### Install Conda
```bash
[admin@vue ~]$ pwd
/home/admin
[admin@vue ~]$ mkdir nannar
[admin@vue ~]$ cd nannar/
[admin@vue nannar]$ mkdir packages
[admin@vue nannar]$ cd packages/
[admin@vue packages]$ ls
[admin@vue packages]$ pwd
/home/admin/nannar/packages
[admin@vue packages]$ curl -O http://gitlab.lab.home:10080/studio/python/Miniconda3-py37_4.8.2-Linux-x86_64.sh
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100 81.1M  100 81.1M    0     0  11.2M      0  0:00:07  0:00:07 --:--:-- 11.3M
[admin@vue packages]$ ls
Miniconda3-py37_4.8.2-Linux-x86_64.sh
[admin@vue packages]$
[admin@vue packages]$ bash Miniconda3-py37_4.8.2-Linux-x86_64.sh

Welcome to Miniconda3 4.8.2

Miniconda3 will now be installed into this location:
/home/admin/miniconda3

  - Press ENTER to confirm the location
  - Press CTRL-C to abort the installation
  - Or specify a different location below

[/home/admin/miniconda3] >>>
PREFIX=/home/admin/miniconda3
Unpacking payload ...
Collecting package metadata (current_repodata.json): done
Solving environment: done


Preparing transaction: done
Executing transaction: done
installation finished.
Do you wish the installer to initialize Miniconda3
by running conda init? [yes|no]
[no] >>> yes
no change     /home/admin/miniconda3/condabin/conda
no change     /home/admin/miniconda3/bin/conda
no change     /home/admin/miniconda3/bin/conda-env
no change     /home/admin/miniconda3/bin/activate
no change     /home/admin/miniconda3/bin/deactivate
no change     /home/admin/miniconda3/etc/profile.d/conda.sh
no change     /home/admin/miniconda3/etc/fish/conf.d/conda.fish
no change     /home/admin/miniconda3/shell/condabin/Conda.psm1
no change     /home/admin/miniconda3/shell/condabin/conda-hook.ps1
no change     /home/admin/miniconda3/lib/python3.7/site-packages/xontrib/conda.xsh
no change     /home/admin/miniconda3/etc/profile.d/conda.csh
modified      /home/admin/.bashrc

==> For changes to take effect, close and re-open your current shell. <==

If you'd prefer that conda's base environment not be activated on startup,
   set the auto_activate_base parameter to false:

conda config --set auto_activate_base false

Thank you for installing Miniconda3!
[admin@vue packages]$


```

Need to re-login

```bash
Last login: Sun Mar 29 01:27:12 2020 from 172.20.0.1
(base) [admin@vue ~]$ ls
miniconda3  nannar
(base) [admin@vue ~]$


(base) [admin@vue ~]$ conda create -n vue
Collecting package metadata (current_repodata.json): done
Solving environment: done


==> WARNING: A newer version of conda exists. <==
  current version: 4.8.2
  latest version: 4.8.3

Please update conda by running

    $ conda update -n base -c defaults conda



## Package Plan ##

  environment location: /home/admin/miniconda3/envs/vue



Proceed ([y]/n)? y

Preparing transaction: done
Verifying transaction: done
Executing transaction: done
#
# To activate this environment, use
#
#     $ conda activate vue
#
# To deactivate an active environment, use
#
#     $ conda deactivate

(base) [admin@vue ~]$ conda activate vue
(vue) [admin@vue ~]$ conda info -e
# conda environments:
#
base                     /home/admin/miniconda3
vue                   *  /home/admin/miniconda3/envs/vue

(vue) [admin@vue ~]$




```



#### Install nvm

```bash

(vue) [admin@vue ~]$ curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100 13527  100 13527    0     0  25943      0 --:--:-- --:--:-- --:--:-- 25913
=> Downloading nvm from git to '/home/admin/.nvm'
=> Cloning into '/home/admin/.nvm'...
remote: Enumerating objects: 290, done.
remote: Counting objects: 100% (290/290), done.
remote: Compressing objects: 100% (257/257), done.
remote: Total 290 (delta 35), reused 97 (delta 20), pack-reused 0
Receiving objects: 100% (290/290), 163.27 KiB | 311.00 KiB/s, done.
Resolving deltas: 100% (35/35), done.
=> Compressing and cleaning up git repository

=> Appending nvm source string to /home/admin/.bashrc
=> Appending bash_completion source string to /home/admin/.bashrc
=> Close and reopen your terminal to start using nvm or run the following to use it now:

export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion
(vue) [admin@vue ~]$

admin@localhost's password:
Last login: Sun Mar 29 01:34:01 2020 from 172.20.0.1
(base) [admin@vue ~]$  nvm ls-remote --lts
         v4.2.0   (LTS: Argon)
         v4.2.1   (LTS: Argon)
         v4.2.2   (LTS: Argon)
         v4.2.3   (LTS: Argon)

       v10.19.0   (Latest LTS: Dubnium)
       v12.13.0   (LTS: Erbium)
       v12.13.1   (LTS: Erbium)
       v12.14.0   (LTS: Erbium)
       v12.14.1   (LTS: Erbium)
       v12.15.0   (LTS: Erbium)
       v12.16.0   (LTS: Erbium)
       v12.16.1   (Latest LTS: Erbium)
(base) [admin@vue ~]$

(base) [admin@vue ~]$ nvm install 12.16.1
Downloading and installing node v12.16.1...
Downloading https://nodejs.org/dist/v12.16.1/node-v12.16.1-linux-x64.tar.gz...
######################################################################## 100.0%
Computing checksum with sha256sum
Checksums matched!
Now using node v12.16.1 (npm v6.13.4)
Creating default alias: default -> 12.16.1 (-> v12.16.1)

(base) [admin@vue ~]$ sudo yum install which

(base) [admin@vue ~]$  which node
/home/admin/.nvm/versions/node/v12.16.1/bin/node
(base) [admin@vue ~]$ which npm
/home/admin/.nvm/versions/node/v12.16.1/bin/npm


```


```bash

npm run dev --port=8090
```

outside localhost:10390

### Install dev tool including g++

```bash
sudo yum group install "Development Tools"

sudo yum group install --skip-broken  "Development Tools"
```


@end
