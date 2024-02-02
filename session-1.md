how to connect linux server?
authentication mechanism
1. what you know = username and password 
2. what you have = tokens
3. what you are = fingerprints,palms,retina


- we can connect linux through ssh
- generally we have public key(like house lock) and private key(key)
- we have to generate publickey and private key 
- linux server is known as server or box or node 
- we have to keep public key in linux server and keep private key with us
- first we have generate key by ssh-keygen -f filename(ITS OUR WISH THE NAME)
- Login into gitbash or windows and go to user folder in c and give the command 
- and there will created public key and private key 
- then create ec2 instance without keypair
- go to keypair option-import keypair in aws
- create security group with inbound rule all traffic
- launch instance and connect
### ssh -i <path-to-private_key> username@ipaddress
## we require public and private key and username and ipaddress and protocal
@ gitbash->ssh-keygen -f filename -> import public key in aws region ->create security group with all inbound traffic --> craete instance --> connect [ssh -i privatekeypath username@publicipaddress]

ssh clients are --> gitbash,putty,mobaxterm
git bash -->ssh client 
ec2 server --> ssh server
ssh --> protocal
22 --> port

### abosolutepath = ssh -i /c/users/dell/daws-76s.pem ec2-user@ip address @ you can know the path by giving pwd command
### relative path = ssh -i <path-to-private_key> username@ipaddress

- $ --> normal user 
- # ---> root user 
- exit --> root to normal
- pwd - present working directory 
- linux home directry= /home/username
- uname = kernal name
- syntax for command ==> <command name> <options> <inputs> 
- <commandname> --help or man <commandname>
- history 
- up arrow and downarrow
- 
- 



