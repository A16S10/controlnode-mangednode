# Automating File Transfers Between Servers Using Ansible


The primary objective of this project was to establish a secure SSH connection between a control node and a managed node, enabling the seamless transfer of files from the management node to desired locations within the managed node. This task was accomplished using two distinct approaches:


Implementation Methods
This task was accomplished using two distinct methods:


Method 1: Ansible Playbook

Playbook Creation:
An Ansible playbook named copyfile.yaml was developed to facilitate the file transfer process. This playbook specifies the source location of the files, the destination path on the managed node, and the ownership settings for the transferred files.


Inventory Configuration:
An inventory file, inventory.ini, was created to detail the managed node's configuration, including the necessary Ansible user credentials. This file serves as a reference for Ansible to identify and connect to the managed node.


Pipeline Execution:
A Jenkins pipeline was utilized to automate the execution of the Ansible playbook, ensuring a streamlined and efficient file transfer process.


Method 2: Ansible Roles


Role-Based Structure:
In the second method, I implemented Ansible roles to organize the tasks according to the project objectives. This approach enhances modularity and reusability of the code.


Task Alignment:
The tasks were aligned within the role structure to ensure clarity and maintainability, allowing for a more systematic execution of the file transfer process.


Alternative Pipeline:
A different Jenkins pipeline was employed for this method, which is documented in the project directory folder, ensuring that the role-based approach is effectively integrated into the deployment workflow.
