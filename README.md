# tomcat_ansible
Ansible Playbook for tomcat installation and configuration.

Things to notice before using the Playbook.
------------------------------------------

1. The download URL is mentioned as a variable in the file `tomcat_ansible/tomcat/tmct/vars/main.yml`. Please check whether the URL is valid or not. If not give the proper URL. Because the URL may change according to the version update.
Variable name is `tomcat_download_url`
2. The tar file name for tomcat is also given as variable for ease of playbook, so please change the tar file name accordingly to the version update or according to the download URL.
Variable name is `tomcat_tar_file_name`
3. The Java Home directory is mentioned as variable. Since the Java Home directory path may vary according to the system. So find your Java Home directory in the system and change the variable accordingly.
Variable name is `JAVA_HOME`
4. Currently the Tomcat is installing on the directory `/opt/tomcat`. You can change it in the variable file as per your requirement. It is optional. It is recommended to install Tomcat on `/opt/` directory.
5. The playbook has been written to choose the custom port for tomcat. The choosen custom port is `9900`. You can change it as per your requirement.
