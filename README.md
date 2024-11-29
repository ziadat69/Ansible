# Ansible <img align="right" alt="Coding" width="50" src="https://fabianlee.org/wp-content/uploads/2017/06/ansible_logo.png">


1) Ad-Hoc Commands: Install Ansible, configure the hosts file, display Yum repository lists, install OpenSSH, manage OpenSSH with the Yum module (install or remove), create files with specific permissions, and delete created files.

2) Playbooks: Create and delete a file with specific permissions, organize and execute multiple playbooks within a main playbook, create groups and add users, and import these playbooks within a main playbook.

 3) Handlers: Install and start services like Apache using handlers, create playbooks with handlers that continue on error and execute multiple tasks.
    
 4) Roles: Create structured tasks for specific purposes such as managing files, users, and server configurations; define handlers within roles to perform additional actions when notified.

5) Vars: Define and use variables within playbooks for dynamic task management, create roles that include variables for flexibility and reusability, and pass variables to playbooks at runtime for dynamic configuration.

6) Loops: Use loops in playbooks to perform repetitive tasks, such as copying or moving multiple files. Define a list of items with source and destination paths and iterate over them to apply actions across multiple files. Customize loop behavior with loop_control for better control over variable names and iterations

7) Conditionals: Use conditionals to execute tasks based on specific conditions, such as checking the status of services or the output of commands. Register results of tasks and use them in subsequent tasks to create dependencies and conditional workflows. Utilize facts to make decisions based on system information, and implement handlers to respond to changes triggered by conditional tasks.
   
8) Blocks: Use task blocks to group tasks together and define rescue and always sections to handle errors and ensure certain tasks are always executed. This helps manage complex workflows and ensures reliability by defining specific actions to take when errors occur and actions to always perform regardless of success or failure of the main tasks.


9) Ansible Vault: Secure sensitive information, such as passwords, within playbooks and roles using Ansible Vault. Define variables with sensitive data and encrypt these variables to ensure secure handling. Utilize Vault-encrypted files in playbooks and roles, and decrypt them during playbook execution to maintain the confidentiality of sensitive information.

10) Ansible Galaxy: A pre-built Ansible role was downloaded from Ansible Galaxy to automatically install and configure Apache. A playbook was then created to utilize the downloaded role, and the target servers were defined in a hosts file. After running the playbook, it was successfully verified that Apache was installed and running on the local system.
