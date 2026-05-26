# Computação Serverless e Ferramentas de Interação

Conceitos sobre execução de código sem servidor e métodos de comunicação com as APIs da AWS.

## ⚡ AWS Lambda
* **O que é:** Serviço de computação serverless orientado a eventos que executa seu código em resposta a gatilhos (como uploads no S3 ou alterações no DynamoDB) e gerencia automaticamente os recursos computacionais subjacentes.
* **Características Práticas:**
  * Você paga apenas pelo tempo de computação que consome (medido em milissegundos).
  * Execução máxima de até 15 minutos por invocação.

## 🛠️ AWS CLI e SDKs
* **AWS CLI (Command Line Interface):** Ferramenta unificada para gerenciar seus serviços AWS a partir da linha de comando, permitindo a automação de tarefas por meio de scripts.
* **AWS SDKs (Software Development Kits):** Bibliotecas específicas por linguagem (como `boto3` para Python) que facilitam a integração dos serviços da AWS diretamente no código da sua aplicação.

---
*💡 Dica de Prova: Funções Lambda são stateless. Qualquer estado ou dado persistente deve ser armazenado fora da função (ex: no S3 ou DynamoDB). Entenda bem quando usar chamadas via SDK dentro da lógica do seu app vs. automações diretas via CLI.*
