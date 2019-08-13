# ftps-server

1. clone repo
2. add certs to target server at /etc/vsftpd/ssl/*cert name in vsftpd.conf.j2
3. Set up ansible hosts ensuring become_user is true.
4. Run ansible-playbook using an example role file:
- hosts: ftps1
  roles:
   - ftps-server
5. Add user and password to target server, ensuring it is in the whitelist too.
