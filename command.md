# ping command
  ansible all -i myhosts -m ping
# playbook execution
  ansible-playbook -i myhosts .yml
# playbook syntax check
  ansible-playbook -i myhosts .yml --syntax-check
# Ad-hoc command
  ansible all -i myhost -b -m apt -a "name=tree"
# filter command
  ansible all -i myhosts -m setup -a "filter=*family*"
  ansible all -i myhosts -m setup -a "filter=*address*"
# java version check in nodes
  alternatives --config java
# listening port command
  netstat -ntulp
# skip tag tasks
  ansible-playbook -i myhosts .yml --skip-tags="name"
  ansible-playbook -i myhosts tags.yml --skip-tags "1st"
# execute tag tasks
  ansible-playbook -i myhosts .yml --tags="name"
  ansible-playbook -i myhosts tags.yml --tags "1st"

  jingar