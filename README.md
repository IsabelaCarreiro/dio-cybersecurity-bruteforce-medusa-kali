dio-cybersecurity-bruteforce-medusa-kali

Laboratório de cibersegurança utilizando Kali Linux e Medusa para realização de ataques de força bruta controlados em ambientes vulneráveis, como FTP, SMB e DVWA, com documentação detalhada e medidas de mitigação.

📌 Objetivo do Projeto

Este laboratório tem como finalidade:

Demonstrar ataques de força bruta utilizando a ferramenta Medusa.

Explorar diferentes serviços vulneráveis (FTP, SMB e DVWA).

Entender como funcionam ataques reais em ambientes controlados.

Aplicar medidas de segurança e endurecimento após a exploração.

🧰 Ferramentas Utilizadas

Kali Linux

Medusa

DVWA (Damn Vulnerable Web Application)

Wordlists (rockyou.txt ou personalizadas)

FTP/Samba vulneráveis

🧪 Cenários Testados
🔹 1. Ataque de força bruta no FTP

Uso do Medusa para quebrar credenciais.

Testes com wordlists personalizadas.

Logs e evidências do ataque.

🔹 2. Ataque de força bruta no SMB

Exploração de compartilhamentos vulneráveis.

Captura de logins válidos via wordlists.

🔹 3. Ataque no DVWA

Bruteforce via módulos do Medusa.

Cenário com nível Low de segurança.

Evidência da captura de credenciais válidas.

📝 Exemplos de Comandos Utilizados
🔐 Força bruta FTP
medusa -h 192.168.0.10 -u admin -P wordlist.txt -M ftp

📁 Força bruta SMB
medusa -h 192.168.0.10 -u guest -P wordlist.txt -M smbnt

🌐 Força bruta DVWA
medusa -h 192.168.0.10 -u admin -P wordlist.txt -M web-form -m FORM:"http://192.168.0.10/login.php"

🛡️ Medidas de Mitigação

Após o ataque, foram aplicadas práticas de segurança como:

Configurar políticas de bloqueio após tentativas inválidas.

Utilizar senhas fortes e políticas de expiração.

Elevar o nível de segurança do DVWA.

Instalação de firewall e fail2ban.

Desabilitar serviços não utilizados.

Monitoramento contínuo com logs.
