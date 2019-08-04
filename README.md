Role Name
=========

Role com propósito de instalar e configurar o fail2ban no CentOS 7.x para proteção ssh.

Role Variables
--------------

Esta role utiliza a variável ```fail2ban_ignoreips``` para especificar os IPs que precisam ser ignorados pelo filtro do fail2ban.

Exemplo de uso:

```
fail2ban_ignoreips:
  - 192.168.0.0/24
  - 192.168.0.1/24
  - 10.10.10.2/32
```



Example Playbook
----------------

Como utilizar essa role na sua playbook.

    - hosts: all
      roles:
         - fail2ban

License
-------

BSD

Author Information
------------------

LinkedIn: https://br.linkedin.com/in/ewertonsilva00
