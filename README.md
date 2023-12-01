# CS320 Final Project Playbook

## Prerequisites

- Verify that your Ansible controller is functioning correctly
- Install the `ansible.windows` and `chocolatey.chocolatey`collections using:
```
ansible-galaxy collection install ansible.windows chocolatey.chocolatey
```

## Running the playbook

- Start by cloning the repository using `git clone`
- Edit the `inventory`` file in the playbook root to match your own hosts. Make sure to test communication with these hosts
- You can select which roles you want to run by editing the `main.yml` file at the playbook root
- Navigate to the root of the playbook repository if you are not already there
- Run the playbook using
```
ansible-playbook -i inventory main.yml
```