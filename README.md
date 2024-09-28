![ANSIBLE_-_AWS_EC2_tags](https://github.com/user-attachments/assets/15fd26de-184b-4423-87f9-daf7444799b5)

# Usage
This project connects your AWS with your Ansible through tags,<br>
you can install services, sceduale reboots and change managed EC2's instances!

# Pre-installation
![image](https://github.com/user-attachments/assets/a69e4ada-2189-479d-80bb-4316d158f3a4)

# Notes
- You will need your pem key, ansible.cfg, manage-ec2.yaml
- Don't forget to update your path to the private key in ansible.cfg
- Change the managed tag in both aws instance tags and inside of the working_after_exam.yaml file - line 11
- Configure your aws cli with keys and region (us-east-1)

Tags Example: (Key | Value):<br>
Name | yoram-ansible-2<br>
Managed | True:Yoram<br>
Service | mysql-server<br>
Version | 8.0.39-0ubuntu0.24.04.2<br>
Restart | */30 * * * *<br>

# Run
```bash
ansible-playbook manage-ec2.yaml
```

# Credits
### Yoram Izilov
