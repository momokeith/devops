# devops

## Deploying bewamo-ui
```
ansible-playbook deploy_bewamo_ui.yml --extra-vars "artifact_path=/tmp/bewamo-ui artifact_id=123654 tag_name=staging"
ansible-playbook deploy_bewamo_ui_test.yml -i hosts.yml --extra-vars "artifact_path=/tmp/bewamo-ui artifact_id=123654"
```