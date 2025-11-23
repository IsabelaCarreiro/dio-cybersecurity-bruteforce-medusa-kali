# Configuração do Ambiente no VirtualBox

## 1. VMs utilizadas
- Kali Linux
- Metasploitable 2

## 2. Modo de Rede
As duas máquinas devem estar configuradas na mesma rede **Host-Only**.

### Como configurar:
1. Abra o VirtualBox
2. Selecione **Kali Linux → Configurações → Rede**
3. Em “Placa 1”, selecione:
   - **Habilitar placa de rede**
   - Conectado a: **Rede somente hospedeiro (Host-Only Adapter)**
4. Repita o procedimento para a VM **Metasploitable 2**

## 3. Verificando IPs
Após iniciar ambas as VMs:

### No Kali:
