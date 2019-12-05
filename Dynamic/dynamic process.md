### STAGE1 - CONFIGURE ANSIBLE ###
1) install ansible on ubuntu 16.04 
  # apt-get update
  # apt-add-repository ppa:ansible/ansible
  # apt-get update
  # apt-get install ansible
  # ansible --version

2) create user (maha)
  # adduser maha

3) we make maha user as a sudo user
  #  visudo
     maha ALL=(ALL) NOPASSWD: ALL
     :wq!

4) we have to connect to nodes  with out pem file.
  # vi /etc/ssh/sshd_config
    PasswordAuthentication yes
   :wq!
  # service ssh restart

### STAGE2 ###
1) Create IAM user 
2) Create AMI with ansible node
3) install pip on ansible master as root user

   #  apt-get install python-pip
   #  pip intall boto
4) Configure IAM user in ansible master as root user
   vi .boto
       #[Credentials]
       #aws_access_key_id = foo
       #aws_secret_access_key = bar
   :wq!
 5) write playbook for create ansible hosts in AWS as ansible user
   
     $ create playbook by using ec2 module as below


