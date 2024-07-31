PP test task

запуск через вызов:
ansible-playbook -i 10.10.0.125, main.yml --ask-vault-password -e "ansible_python_interpreter=/usr/bin/python3"

***
1. испытано на debian 11.10
2. пароль к vault направлен отдельно
3. все переменные находятся в group_vars
4. безусловная перезагрузка вызывается в конце общего сценария
5. конфигурация предоставленного nginx.conf проверяется, но ошибка игнорируется