# Configuração do Metasploitable 2

Metasploitable 2 é uma VM vulnerável usada para testes ofensivos.

## 1. Acessando
Usuário padrão:
msfadmin/msfadmin

## 2. Serviços Disponíveis
Para identificar serviços expostos:

No Kali, execute:
nmap -sV 192.168.56.102

Normalmente, aparecem serviços como:

- FTP
- SSH
- Telnet
- SMB
- Apache (Web Server)
- MySQL

## 3. Ativar DVWA
O DVWA já está ativado por padrão e funciona acessando:

http://192.168.56.102/dvwa

Usuário padrão:
admin / password
