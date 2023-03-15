# Information
**Description:** Practice from Ansible course.

**OS:** CentOS 7

# Prepare
Install _roles_ and _collections_:
```
ansible-galaxy install -r requirements.yml
ansible-galaxy collection install -r requirements.yml
```
Then exec playbook:
`ansible-playbook playbook.yml`

# Variables
| Variable | Default Key |
|----------|-------------|
| SECRET_KEY_BASE | secret |
| RAILS_ENV | production |
| RAILS_LOG_TO_STDOUT | 1 |
| DB_HOST | 127.0.0.1 |
| DB_PORT | 5432 |
| DB_NAME | ruby |
| DB_USER | postgres |
| DB_PASSWORD | password |