# Componentes Core: Amazon S3 e Amazon DynamoDB

Resumo focado nos serviços de armazenamento e banco de dados essenciais para o desenvolvedor AWS.

## 🪣 Amazon S3 (Simple Storage Service)
* **O que é:** Serviço de armazenamento de objetos projetado para armazenar e recuperar qualquer quantidade de dados de qualquer lugar.
* **Características para o Desenvolvedor:**
  * Altamente escalável, com durabilidade de 99.999999999% (11 novos).
  * Permite hospedagem de sites estáticos.
  * Suporta controle de versão de objetos para evitar exclusões acidentais.

## ⚡ Amazon DynamoDB
* **O que é:** Banco de dados NoSQL de chave-valor e documentos, totalmente gerenciado, que oferece performance de milissegundos em qualquer escala.
* **Características para o Desenvolvedor:**
  * Tabelas sem esquema rígido (schemaless).
  * Escalonamento automático de leitura e escrita (RCUs e WCUs).
  * Integração nativa com AWS Lambda através do DynamoDB Streams para arquiteturas baseadas em eventos.

---
*💡 Dica de Prova: O S3 é para dados não estruturados (arquivos, imagens, mídias). O DynamoDB é para dados estruturados/semi-estruturados que exigem acessos rápidos de chave-valor com latência previsível.*
