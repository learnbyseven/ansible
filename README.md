# ansible
ANSIBLE WORK
perquisites
1. Ansible package install
2. Password less ssh setup jumpbox and target hosts 
## Steps
sudo ansible-galaxy install nginxinc.nginx
sudo ansible-galaxy install nginxinc.nginx_controller_agent
sudo git clone 
cd ansible 

#ng+ remote install, sample (Provide target hosts entry inside inventory-hosts.yml)
ansible-playbook -i inventory-hosts.yml nginxplus-install-playbook.yaml

#ctr agent install, sample (Use option -e for your enviornment specific variables) 
ansible-playbook -i inventory-hosts.yml myagent-playbook.yml -e "api_key=dfb614c8b56e7098a8e4aff398f656ac"
