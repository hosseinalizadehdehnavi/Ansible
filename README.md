# **Ansible Automation Project**  

## **Overview**  
This Ansible project allows you to automate both simple and complex server configurations **effortlessly**. Instead of performing manual setups, you can execute a **single command** to configure your system efficiently.  

## **Features**  
This project includes various **Roles** for essential system configurations:  

1. **`add_hostname_in_etc`** – Adds the IP addresses from `Inventory/hosts` to the `/etc/hosts` file on target hosts.  
2. **`apt_update_install_package`** – Updates the package cache and installs specified packages.  
3. **`backup`** – Compresses a file and copies the compressed version to a host.  
4. **`change_hostname`** – Changes the system’s hostname.  
5. **`change_timezone`** – Modifies the system timezone.  
6. **`disable_swap`** – Disables and removes swap space.  
7. **`install_node_exporter`** – Installs **Node Exporter** for system monitoring.  
8. **`set_dns`** – Configures the system’s DNS server.  

## **Prerequisites**  
Before using this project, ensure you have:  
- Ansible installed (`ansible --version` to check)  
- A configured `inventory/hosts` file with target servers  
- SSH access to the target machines  

## **Usage**  

```bash
ansible-playbook -i inventory/hosts playbooks/<playbook_name>.yml
```

For example, to update packages and install a package:  

```bash
ansible-playbook -i inventory/hosts playbooks/change_timezone.yml
```
