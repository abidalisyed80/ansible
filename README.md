# ansible
Project Ansible

## Varilables 
*    git_repo_url: "{{ repo_url }}" # Git Repository URL
*    git_branch: "{{ branch_name }}" # Git Branch Name
*    dest_folder: "{{ dest_folder }}" # Destination folder where to pull code

# use 'ansible-playbook' and pass variables  value to playbook, see example below
```bash
ansible-playbook git_clone.yaml -e "repo_url=git@github.com:user_name/repo.git" -e "branch_name=test_branch" dest_folder=/tmp/" 
```

# Similarly see 'docker-imageBuilder.yaml' and pass Env variables as needed
