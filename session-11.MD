## setting up github authentication by key 

- to push code to github we need authentication
- username/password = for this we need to enter frequently
- username/key = it will autoomatically taken from private key and it is very secure
- we place public key in github server and keep private key with us
- we can use already created key
- copy public key- goto settings in github a/c-ssh and gpgkeys-newsshkey-give title-pastekey-addshhkey
- for setup private:
- go to .ssh folder in our local which user directory[/c/users/dell]-config-
- search as  git ssh config syntax in internet
- 
- Host github.com
  HostName github.com
  User git
  PreferredAuthentications publickey
  IdentityFile ~/daws-76s-github 
  # ~ is nothing our home folder

- https://github.com/meenakshichiluveru/ansible.git - username/password
- git@github.com:meenakshichiluveru/ansible.git -privatekey

1. signup for github
2. create public/private key 
3. place public key key in github
4. keep private key 
5. create .ssh folder in home folder
6. create config file without any extensions in .ssh folder
7. Host github.com
  HostName github.com
  User git
  PreferredAuthentications publickey
  IdentityFile ~/daws-76s-github 
8. 
9. # create a folder in local and intiate it with git init-it becomes git folder
10. # git status - it shows status of git repo files
11. # git add -stagingarea/temporary area - it is storing the files before push
12. make sure you give username and email before commit
13. # git commit m "commit message"- we need to inform why we are doing
14. # git remote add origin git@github.com:meenakshichiluveru/ansible.git - informing our local repo about central location
15. # git push origin master 
16. git config --global user.name "meenakshichiluveru"
17. git config --global user.email "meenakshichiluveru9949@gmail.com"
