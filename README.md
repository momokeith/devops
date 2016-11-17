# devops

## Deploying bewamo-ui
```
ansible-playbook deploy_bewamo_ui.yml --extra-vars "artifact_path=/tmp/bewamo-ui artifact_id=123654 tag_name=staging"
ansible-playbook deploy.yml --extra-vars "project_name=bewamo-ui project_type=web artifact_path=/tmp/bewamo-ui artifact_id=123654 tag_name=staging"
ansible-playbook deploy_bewamo_ui_test.yml -i hosts.yml --extra-vars "artifact_path=/tmp/bewamo-ui artifact_id=123654"
ansible-playbook deploy.yml --extra-vars @bewamo-ui.config.json
```