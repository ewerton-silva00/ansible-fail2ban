fail2ban
=========

Role com propósito de instalar e configurar o fail2ban no CentOS 7.x para proteção ssh.

Role Variables
--------------

Esta role utiliza as variáveis abaixo:

```
# Tempo na qual um IP permanecerá banido.
# Valor em segundos.
# 3600 segundos equivale a 1 hora.
fail2ban_bantime: 3600

# Intervalo de tempo em que o fail2ban deve detectar falhas de maxretry.
# Valor em segundos.
# 300 segundos equivale a 5 minutos.
fail2ban_findtime: 300

# Número de tentativas antes de banir um IP.
fail2ban_maxretry: 5

# Lista dos IPs/CIDR ou hostnames que não serão banidos.
# Informar os IPs/CIDR um abaixo do outro.
fail2ban_ignoreips:
  - 127.0.0.1/8
```

> Os valores acima são usados por padrão.

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
