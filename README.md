# ansible_test_tasks

# Start crteate user
ansible-playbook scripts/create_user.yml -e @passwords

# Start iptbles rules
ansible-playbook scripts/iptables.yml -e @passwords

# File content  passwords
ansible_ssh_pass: sshpass
ansible_sudo_pass: sshsudopass
vault_user_pass: UserPass