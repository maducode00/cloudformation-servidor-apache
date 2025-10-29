# 🚀 Projeto AWS CloudFormation – Servidor Apache EC2

Este projeto utiliza **AWS CloudFormation** para automatizar a criação de uma infraestrutura básica na nuvem: uma instância EC2 com Apache configurado automaticamente. É ideal para quem está começando com **Infraestrutura como Código (IaC)** e deseja entender como provisionar recursos na AWS usando templates YAML.

---

## 📦 Recursos Criados

- ✅ Instância EC2 (t2.micro – elegível para Free Tier)
- 🔐 Grupo de Segurança com acesso HTTP (porta 80) e SSH (porta 22)
- 🧰 Apache instalado e configurado via script de inicialização (UserData)
- 🌐 Página web simples servida automaticamente
- 📤 IP público da instância exibido como saída (Output)

---

## 📁 Estrutura do Projeto

projeto-cloudformation/ │
 ├── template.yaml # Template CloudFormation com definição dos recursos └── README.md # Documentação do projeto
 
---

## 🛠️ Como Usar

### 1. Acesse o Console da AWS
Entre em [https://console.aws.amazon.com/cloudformation](https://console.aws.amazon.com/cloudformation)

### 2. Crie uma nova Stack
- Clique em **Create Stack > With new resources (standard)**
- Escolha **Upload a template file**
- Envie o arquivo `template.yaml`

### 3. Avance pelas etapas
- Dê um nome à stack (ex: `ServidorApache`)
- Avance até a tela de revisão e clique em **Create Stack**

### 4. Acesse o servidor
- Vá até a aba **Outputs** da stack
- Copie o **IP público**
- Acesse no navegador: `http://SEU-IP`
- Você verá a página:  
  **“Servidor Web via CloudFormation”**

---

## 🧠 Tecnologias Utilizadas

- **AWS CloudFormation**
- **Amazon EC2**
- **Apache HTTP Server**
- **YAML (Infraestrutura como Código)**

---

## 📈 Possíveis Evoluções

- 🔄 Auto Scaling e Load Balancer
- 🗃️ Integração com RDS ou DynamoDB
- 🧭 VPC personalizada com sub-redes públicas/privadas
- 📦 Modularização com Nested Stacks
- 🚀 Deploy contínuo com AWS CodePipeline
- 📊 Monitoramento com CloudWatch

---

## 👩‍💻 Autora

**Maria**  
Paulista – Pernambuco, Brasil  
Projeto desenvolvido com foco em aprendizado prático de automação de infraestrutura na AWS.

---

## 📄 Licença

Este projeto está sob a licença MIT. Sinta-se livre para usar, modificar e compartilhar.

