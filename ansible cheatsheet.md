
Subsystem sftp internal-sftp or 
[test]
hostname.com.cn  ansible_connection=ssh

ansible <host> -i <inventory-file> -m <module>

ansible all -m ping 

ansible all -u "jiazhu3" -k -a "hostname"

ansible all -u "jiazhu3" -k --sudo -K       -a "cat /etc/ssh/sshd_config"

ansible myhost --sudo -m raw -a "yum install -y python2 python-simplejson"
