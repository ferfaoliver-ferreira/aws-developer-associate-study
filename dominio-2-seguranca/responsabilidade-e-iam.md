# Modelo de Responsabilidade Compartilhada e IAM

Fundamentos de governança, controle de acesso e divisão de responsabilidades de segurança.

## 🤝 Modelo de Responsabilidade Compartilhada
* **Segurança DA Nuvem (Responsabilidade da AWS):** A AWS protege a infraestrutura global que executa todos os serviços (hardware, software, redes e facilidades físicas dos data centers).
* **Segurança NA Nuvem (Responsabilidade do Cliente):** O cliente gerencia a configuração dos serviços, criptografia de dados, sistemas operacionais das instâncias, segurança de rede (firewalls) e gerenciamento de identidades (IAM).

## 🔑 AWS IAM (Identity and Access Management)
* Permite controlar o acesso aos recursos da AWS de forma segura.
* **Princípio do Menor Privilégio:** Conceder apenas as permissões estritamente necessárias para que um usuário ou serviço execute sua função.
* Utilização de Usuários, Grupos, Políticas (JSON) e Roles (Funções assumidas por serviços, como dar permissão para o Lambda ler o S3).

---
*💡 Dica de Prova: Se a questão falar sobre atualizar o patch do Sistema Operacional de uma EC2 ou configurar regras de criptografia no S3, a responsabilidade é do **Cliente**. Se falar sobre quebra física de disco ou segurança física do data center, é da **AWS**.*
