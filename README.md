# Ansible Case Study - Apache, Nginx & Java Configuration

**Step 1:** Create two server groups in the inventory.ini file

- Add the IP addresses of Apache and Nginx servers.

**Step 2:** Create two Ansible roles named apache and nginx

**Step 3:** Configure the apache role

- Add tasks to install Apache, copy HTML file, and start the service in roles/apache/tasks/main.yml, refer configure.yml and install.yml in tasks

- Place the HTML file sample.html in roles/apache/files/.

**Step 4:** Configure the nginx role

- Add tasks to install Nginx, copy HTML file, and start the service in roles/nginx/tasks/main.yml, refer configure.yml and install.yml in tasks

- Place the HTML file sample.html in roles/nginx/files/.

**Step 5:** Create a java role to install Java on Apache servers

- Define the task to install Java in roles/java/tasks/main.yml.

**Step 6:** Create playbook.yml to run all the configurations

- Include apache, nginx, and java roles in playbook.yml.

**Step 7:** Run the Ansible Playbook

**Step 8:** Verify Installation on Slave Groups

- Access the web pages for Apache and Nginx:
  
  - http://<apache_server_ip>/
    
  - http://<nginx_server_ip>/
 
- Check Java version on Apache servers: java --version

 

