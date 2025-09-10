# desafioinstanciasEC2
Resumo do aprendizado adquirido até aqui
# 🚀 Desafio EC2 na AWS - DIO

## 📚 Sobre
Este repositório documenta o desafio prático de **gerenciamento de instâncias EC2 na AWS**, parte da trilha de formação em computação em nuvem da DIO. A proposta é consolidar os conhecimentos adquiridos durante as aulas por meio da criação, configuração e gerenciamento de uma instância EC2, além da documentação técnica dessa experiência.

## 🧠 Aprendizados Aplicados

### 1. Introdução à AWS
- Compreensão dos modelos de serviço (IaaS, PaaS, SaaS)
- Vantagens da computação em nuvem

### 2. Fundamentos de Infraestrutura
- Escolha de região e zona de disponibilidade
- Conceito de VPC, subnets e grupos de segurança

### 3. Segurança na Conta AWS
- Criação de usuários IAM
- Ativação do MFA
- Boas práticas para proteção da conta root

### 4. Acesso Seguro e Custos
- Uso de alertas de orçamento (AWS Budgets)
- Controle de custos com instância `t2.micro` (Free Tier)

### 5. Instâncias EC2
- Criação e configuração de uma instância EC2
- Acesso remoto via SSH
- Instalação de serviços na máquina virtual

### 6. Armazenamento EBS e S3
- Volume EBS para armazenamento em bloco
- Introdução ao S3 como armazenamento de objetos

### 7. Gerenciamento de Instâncias
- Comandos para iniciar, parar e encerrar instâncias EC2
- Alterações de estado e tipos de instância

### 8. Snapshots
- Criação de snapshots de volumes EBS como backup

---

## 💻 Etapas da Prática Realizada

1. Acesso ao console da AWS
2. Criação de uma instância EC2 (Amazon Linux 2023)
3. Configuração de grupo de segurança com acesso via SSH e HTTP
4. Conexão à instância via SSH
5. Instalação do NGINX
6. Acesso à aplicação pelo navegador
7. Criação de snapshot do volume EBS

---

## 📜 Comandos Utilizados

```bash
# Conectar via SSH
ssh -i "minha-chave.pem" ec2-user@<IP-PUBLICO>

# Atualizar pacotes e instalar NGINX
sudo yum update -y
sudo amazon-linux-extras install nginx1 -y
sudo systemctl start nginx
sudo systemctl enable nginx


