# ANSIBLE ROLE DOCKER, JENKINS, GITLAB
-------------------------
## Installs Docker, Jenkins, Gitlab for Ubuntu linux servers.
## Requirements
-------------------------
        OS: Ubuntu (16.04/18.04/20.04)
    Storage: The Omnibus GitLab package requires about 2.5 GB of storage space for installation.
    CPU: 4 cores is the recommended minimum number of cores and supports up to 500 users, 8 cores supports up to 1000 users
    Memory: 
      4GB RAM is the required minimum memory size and supports up to 500 users (Our Memory Team is working to reduce the memory requirement).
      8GB RAM supports up to 1000 user

## Role Variables
-------------- 
    ---
    # vars file for roles
        default_container_image: jenkins/jenkins:lts 

## Dependencies
------------
    None.

## Example Playbook
----------------
    ---
    - name: Install Jenkins & Gitlab
      hosts: linux
      become: true  
      roles:
        - role-docker
        - role-jenkins
        - role-gitlab 
       
## License
-------
    LÊ NGỌC HIẾU

## Author Information
------------------

    This role was created in 2022 by Lê Ngọc Hiếu from Việt Nam, Devops Engineer

