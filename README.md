# Информация
**Цель:** Закрепление материала полученного в курсе Ansible, получение практического опыта написания и использования ролей.

**Результат:** Работающая инфраструктура для приложения. Репозиторий на Github.com с ролями и плейбуками Ansible.

**Задание:** Необходимо подготовить сервер для работы приложения на основе ОС Centos 7.

**ОС:** CentOS 7 (https://app.vagrantup.com/generic/boxes/centos7/versions/4.2.14)

# Подготовка
Перед выполнением плейбука установите роли и коллекции командами:
```
ansible-galaxy install -r requirements.yml
ansible-galaxy collection install -r requirements.yml
```
Затем запустите плейбук:
```
ansible-playbook playbook.yml
```

# Переменные
| Название | Ключ по умолчанию |
|----------|-------------------|
| SECRET_KEY_BASE | secret |
| RAILS_ENV | production |
| RAILS_LOG_TO_STDOUT | 1 |
| DB_HOST | 127.0.0.1 |
| DB_PORT | 5432 |
| DB_NAME | ruby |
| DB_USER | postgres |
| DB_PASSWORD | password |