# ansible_nginx_balancer
nginx_balansir - role for nginx balancer host  
nginx_webapp - role for app hosts
# requirements
was tested on cenos6 distr
#role variables
ip1, ip2 - web app hosts ip adresses
# examples
 – hosts: web_balansir   
  vars:  
  – ip1: x.x.x.x  
  – ip2: x.x.x.x  
  roles:  
  – role:  nginx_balansir  
  tags:  
– nginx_balansir  
– hosts: web_app  
roles:  
   – role: nginx_webapp  
   tags:  
– webapp  
###### inventory file
[web_balansir]  
[web_app]
