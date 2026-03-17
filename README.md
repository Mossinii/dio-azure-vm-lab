# ☁️ Deploy de Infraestrutura Linux na Azure (Ubuntu Server)

## 📌 Visão Geral do Projeto
Este repositório documenta o provisionamento de uma Máquina Virtual (VM) na Microsoft Azure para o desafio da DIO. O foco foi aplicar boas práticas de governança, segurança de rede e conectividade remota via SSH.

## 🛠️ Especificações Técnicas
- **Máquina:** Standard D2s v3 (2 vCPUs, 8 GiB RAM)
- **Sistema Operacional:** Ubuntu Server 24.04 LTS (x64)
- **Localização:** West US
- **Segurança:** Autenticação via par de chaves RSA (SSH)
- **Network Security Group (NSG):** Porta 22 (SSH) liberada para administração.

## 🛡️ Diferenciais de Implementação (NETZ Strategy)
- **Higiene de Nuvem:** Configuração de exclusão automática de IP público e placa de rede (NIC) ao deletar a VM para evitar custos residuais.
- **Resolução de Problemas:** Adaptação de SKU (de B1s para D2s v3) para contornar limitações de cota regional, garantindo a entrega do projeto.
- **Segurança:** Desativação de login por senha, utilizando exclusivamente chaves criptográficas.

## 📸 Evidências do Projeto

### 1. Provisionamento Concluído
![Painel Azure](./02-vm-config.png)

### 2. Conectividade e Acesso Remoto (SSH)
![Acesso Terminal](./03-access-ssh.png)
> Como demonstrado na imagem, o acesso foi realizado com sucesso via terminal, confirmando a integridade das regras de firewall e chaves de segurança.

---
🚀 *Projeto desenvolvido por Kauan - Foco em Cloud & Infraestrutura NETZ.*
