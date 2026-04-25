# Preps

## Prepare ansible host

- Make sure you can connect to all other hosts with a user with sudo privilleges
  **Note** If all users have the same username and password (e.. ldap auth), you can do without ssh keys.
  If not, alsoe setup passwordless authentication with ssh keys
- Make sure that all nodes (ansible, db hosts and backup server) can resolve eachother using either DNS or /etc/hosts
- Prepare the ansible host
  ```bash
  curl https://raw.githubusercontent.com/pgvillage/pgv_azure/main/bootstrap_debian.sh | sudo bash
  ```
- setup inventory (~/git/pgv_kvm/environments/cluster1/hosts)
  - set proper hosts and proper ip adresses
