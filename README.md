# aws-developer-associate-study
Repositório de estudos para a certificação AWS DVA-C02
# ☁️ AWS Certified Developer – Associate (DVA-C02) - Guia de Estudos

Este repositório foi criado com o objetivo exclusivo de centralizar, organizar e documentar toda a preparação teórica para o exame de certificação **AWS Certified Developer - Associate**. Aqui se encontram resumos detalhados, mapas mentais dos conceitos-chave e fichamentos focados nos critérios do guia oficial da prova.

## 🎯 Objetivo
- Consolidar a base teórica exigida para o ecossistema AWS (desenvolvimento, segurança, implantação e otimização).
- Mapear pegadinhas comuns de prova e dicas de cenários arquiteturais.
- Servir como um guia de consulta rápida para revisão antes do exame AWS DVA-C02.

---

## 🗺️ Cobertura dos Domínios do Exame

| Domínio | Descrição | Status de Revisão |
| :--- | :--- | :---: |
| **Domínio 1** | Desenvolvimento com Serviços AWS (Fundamentos, S3, DynamoDB, Lambda, SDKs) | ⏳ Em Progresso |
| **Domínio 2** | Segurança (IAM, KMS, Secrets Manager, Parameter Store, Cognito, ACM) | ⏳ Em Progresso |
| **Domínio 3** | Implantação e Monitoramento (CI/CD, CloudFormation, CloudWatch, X-Ray) | ⚪ Não Iniciado |
| **Domínio 4** | Refatoração e Otimização (SQS, SNS, Kinesis, Estratégias de Caching) | ⚪ Não Iniciado |

---

## 🚀 Conteúdos Documentados

### 🛠️ Domínio 1: Desenvolvimento com Serviços AWS
Foco nos conceitos estruturais e nas ferramentas de interação com a nuvem:
* **Infraestrutura Global da AWS:** Entendimento de Regiões, Zonas de Disponibilidade (AZs) e o modelo de faturamento sob demanda (*pay-as-you-go*).
* **Componentes Principais de Arquitetura:** Modelos escaláveis utilizando serviços essenciais como **AWS Lambda** (computação Serverless), **Amazon DynamoDB** (banco de dados NoSQL de alta performance) e **Amazon S3** (armazenamento de objetos).
* **Interface e Automação:** Diferenças conceituais e aplicações práticas do uso do AWS CLI e SDKs na integração de sistemas.

### 🔐 Domínio 2: Segurança e Gerenciamento de Segredos
Conceitos vitais sobre proteção de dados e identidades sob a ótica do desenvolvedor:
* **Modelo de Responsabilidade Compartilhada:** Fixação do princípio de que a AWS é responsável pela segurança *da* nuvem e o cliente pela segurança *na* nuvem.
* **Criptografia e Chaves:** Uso do **AWS KMS** e do **AWS CloudHSM** para controle e gerenciamento de chaves de criptografia para dados em repouso e em trânsito (utilizando **ACM** para certificados SSL/TLS).
* **Gerenciamento de Credenciais:**
  * *AWS Secrets Manager:* Armazenamento e rotação automática de segredos complexos (como credenciais de bancos de dados).
  * *Systems Manager (SSM) Parameter Store:* Gerenciamento centralizado e hierárquico de parâmetros de configuração e segredos simples.
* **Proteção e Classificação de Dados:** Métodos para identificação de dados sensíveis (**PII** - Informações Pessoais Identificáveis e **PHI** - Dados de Saúde) e a aplicação de técnicas de mascaramento ou exclusão.

---

## 📚 Metodologia e Materiais de Apoio
- Resumos estruturados por tópicos, com base de materiais de estudos da EDN e das documentações da AWS (Domínios 1 e 2).
- Mapas mentais focados nos fluxos de serviços e arquiteturas do exame.
- Caderno de erros de simulados técnicos.

---
*💡 Dica de exame monitorada: "O KMS suporta apenas chaves simétricas para criptografia do CloudWatch Logs. Atente-se à diferença exata de cenários entre Secrets Manager (com rotação) e Parameter Store (sem rotação nativa de credenciais) nas questões de múltipla escolha!"*
