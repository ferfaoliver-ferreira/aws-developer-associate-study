# Gerenciamento de Segredos e Classificação de Dados Sensíveis

Estratégias de armazenamento seguro de variáveis de ambiente, credenciais e governança de dados privados.

## 🤫 AWS Secrets Manager vs. Systems Manager Parameter Store
* **AWS Secrets Manager:**
  * Desenvolvido especificamente para gerenciar segredos complexos (senhas de bancos de dados, chaves de API).
  * Recursos avançados: **Rotação automática de segredos** integrada (ex: altera a senha no RDS automaticamente).
  * Custo associado por segredo armazenado.
* **Systems Manager (SSM) Parameter Store:**
  * Repositório centralizado para strings de configuração, URLs e dados em texto puro ou criptografados (SecureString).
  * Não possui rotação automática nativa de credenciais externas.
  * Geralmente usado para parâmetros gerais de aplicações.

## 🔍 Classificação e Sanitização de Dados
* Identificação de dados críticos:
  * **PII (Informações Pessoais Identificáveis):** CPF, e-mail, nomes.
  * **PHI (Dados de Saúde):** Prontuários, históricos médicos.
* Aplicação de técnicas de **mascaramento** ou exclusão seletiva antes do armazenamento definitivo para garantir conformidade e proteção à privacidade.

---
*💡 Dica de Prova: Se a questão exigir **rotação automática de credenciais de banco de dados**, a resposta correta será **AWS Secrets Manager**. Se exigir apenas uma forma hierárquica e gratuita/barata de guardar parâmetros gerais de configuração, a resposta será **Parameter Store**.*
