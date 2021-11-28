# UdacityCloudArchitect

### Notes
Git Bash is not working with Password and https.

$ git remote -v
origin  https://github.com/programmingkitchen/UdacityCloudArchitect.git (fetch)
origin  https://github.com/programmingkitchen/UdacityCloudArchitect.git (push)

# Git Config
Local

Before
$ git remote -v
origin  https://github.com/programmingkitchen/UdacityCloudArchitect.git (fetch)
origin  https://github.com/programmingkitchen/UdacityCloudArchitect.git (push)

After
$ git remote -v
origin  git@github.com/programmingkitchen/UdacityCloudArchitect.git (fetch)
origin  git@github.com/programmingkitchen/UdacityCloudArchitect.git (push)

SSH Keys
git remote set-url origin git@github.com:USERNAME/REPOSITORY.git
git remote set-url origin git@github.com:programmingkitchen/UdacityCloudArchitect.git



Config
rgran@HPPAVILION-1 MINGW64 ~/.ssh
$ pwd
/c/Users/rgran/.ssh

rgran@HPPAVILION-1 MINGW64 ~/.ssh
$ ls
config  id_rsa  id_rsa.pub  id_rsa_github  id_rsa_github.pub  known_hosts


Config File
rgran@HPPAVILION-1 MINGW64 ~/.ssh
$ cat config
Host 10.*
        StrictHostKeyChecking no
        UserKnownHostsFile=/dev/null
Host github.com
  HostName github.com
  IdentitiesOnly yes
  IdentityFile ~/.ssh/id_rsa_github
  user git
