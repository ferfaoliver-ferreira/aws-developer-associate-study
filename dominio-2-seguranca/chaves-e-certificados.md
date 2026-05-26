# Criptografia, Chaves e Certificados de Rede

Conceitos de proteção de dados em repouso (at rest) e em trânsito (in transit).

## 🔑 Proteção de Dados
* **Em Repouso:** Dados salvos em disco (S3, EBS, DynamoDB). Protegidos com criptografia baseada em chaves.
* **Em Trânsito:** Dados trafegando pela rede. Protegidos através de protocolos criptográficos seguros como TLS/SSL.

## 🛠️ Serviços de Gerenciamento
* **AWS KMS (Key Management Service):** Serviço gerenciado que facilita a criação e o controle de chaves criptográficas. Cobre chaves simétricas e assimétricas, integrando-se nativamente à maioria dos serviços AWS.
* **AWS CloudHSM:** Módulos de segurança de hardware (HSMs) dedicados e validados na nuvem AWS para clientes que exigem controle total e exclusivo sobre suas chaves por questões normativas rígidas.
* **AWS Certificate Manager (ACM):** Provisiona, gerencia e implanta certificados SSL/TLS públicos e privados para uso com serviços da AWS (como CloudFront e Application Load Balancers).

---
*💡 Dica de Prova: O **KMS suporta apenas chaves simétricas para criptografia do CloudWatch Logs**. Guarde essa regra! O CloudHSM é escolhido apenas quando há uma exigência estrita de conformidade de hardware dedicado, caso contrário, o KMS é a opção padrão ideal.*
