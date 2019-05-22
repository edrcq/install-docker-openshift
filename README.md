# install docker and openshift on your centos 7 VM
Fork and clone this repository
 
Change the inventory file accordingly to your architecture
and hit
 
```ansible-playbook -i inventory playbook.yml```

When it's all is done 

ssh to your virtual machine and get your public IP address 
and hit

``` oc cluster public-hostname=<your_public_ip_address> up ```

Log on as system:admin on your VM 

``` https://<your_public_ip_address>:8443 ```

By-pass the SSL credentials verifications