# devops

## Deploying bewamo-ui
```
ansible-playbook deploy.yml --extra-vars "project_name=bewamo-ui tag_name=staging"
ansible-playbook deploy_bewamo_ui_test.yml -i hosts.yml
```