Ссылка на задание - https://github.com/PeacockTeam/new-job/blob/master/DevOps%20Ansible

Один шаг который я делал без ансибла это помещение публичного ключа(пользователя под которым работает ансибл) с первой vm в sshd папку на второй vm.
В итоге команда:
> ansible-playbook -i hosts -b deploy_ldap.yml

в команде указание на инвентарь hosts и плэйбук (для удобства все переменные и таски лежат в одном playbook файле)

Скриншот результата. (Шаги с добавлением зелёные потому что не первый запуск скрипта)
![image](https://github.com/Naverx/Ansible_ldap/assets/14109161/c8138269-5a27-4da3-8ed1-53513279bfe4)


Пример скриншотов со второй машины куда был установлен Openldap
![image](https://github.com/Naverx/Ansible_ldap/assets/14109161/fd9d1265-cb2f-463d-9989-603162f28516)
![image](https://github.com/Naverx/Ansible_ldap/assets/14109161/e72cd04f-ee4f-41ad-a1d2-54fb129ef75e)
