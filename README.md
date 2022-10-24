# ansible-playbook deploy-apache.yaml --extra-vars “apache_listen_port=8080 apache_listen_port_ssl=443”

Before running a playbook with a single-host solution user providedterraform files to create a single VM and specify the values of ```ansible_host``` and ```php_server_internal_ip``` variables in ```single_host``` hosts file.  
To run a playbook for a single-host deployment:
```
ansible-playbook -i single_host main.yaml -vv
```
