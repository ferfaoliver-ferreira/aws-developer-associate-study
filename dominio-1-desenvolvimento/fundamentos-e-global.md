# Fundamentos da Nuvem e Infraestrutura Global

Este resumo aborda os conceitos iniciais sobre como a infraestrutura global da AWS está organizada e como o modelo de computação impacta o desenvolvimento de aplicações.

Estes materiais didáticos fornecem uma preparação técnica abrangente para a certificação AWS Certified Developer – Associate. O conteúdo inicial detalha os fundamentos da computação em nuvem, explicando modelos de implantação, a infraestrutura global da Amazon e o sistema de faturamento sob demanda. Os documentos avançam para conceitos de desenvolvimento, segurança cibernética e estratégias de automação para a entrega de softwares. Além da teoria, as fontes incluem exercícios práticos e simulados que abordam serviços essenciais como Lambda, DynamoDB e S3. O objetivo central é capacitar o estudante a projetar arquiteturas escaláveis, resilientes e otimizadas dentro do ecossistema AWS.

# 🌐 Fundamentos da AWS e Infraestrutura Global

Antes de mergulhar no desenvolvimento, é essencial compreender os pilares estruturais da AWS. Este conhecimento é a base para responder questões de cenários arquiteturais na prova.

---

### 🏛️ Modelos de Implantação
* **On-Premises (Local):** Infraestrutura própria com altos custos iniciais (CapEx) e manutenção física contínua.
* **Nuvem (Cloud):** Recursos 100% sob demanda com gastos operacionais (OpEx) flexíveis.
* **Híbrida:** Modelo que combina e conecta a infraestrutura local com o ambiente de nuvem da AWS.

---

### 💰 Benefícios Práticos da Nuvem
* **Pay-as-you-go:** Você é cobrado exclusivamente pelo que consome e pelo tempo real de uso.
* **Elasticidade:** Capacidade do sistema de se adaptar automaticamente (adquirindo ou liberando recursos) conforme a oscilação imediata da demanda.
* **Escalabilidade:** Capacidade da arquitetura de suportar o crescimento do volume de trabalho:
  * *Horizontal (Scaling Out/In):* Adicionar ou remover instâncias (ex: mais servidores).
  * *Vertical (Scaling Up/Down):* Aumentar ou diminuir o poder de uma instância existente (ex: mais RAM ou CPU).

---

### 🗺️ Infraestrutura Global da AWS
* **Regiões:** Áreas geográficas isoladas ao redor do mundo que hospedam múltiplos data centers.
* **Zonas de Disponibilidade (AZs):** Clusters de data centers discretos e redundantes dentro de uma Região, projetados para garantir **Alta Disponibilidade** e tolerância a falhas.
* **Edge Locations:** Pontos de presença globais distribuídos estrategicamente para fazer o cache de conteúdo estático e dinâmico mais próximo do usuário final via **Amazon CloudFront**.

---

### 🤝 Modelo de Responsabilidade Compartilhada

A divisão de tarefas de segurança é um dos tópicos mais recorrentes no exame. Lembre-se da regra de ouro:

> 🔒 **Segurança DA Nuvem (Responsabilidade da AWS):** Proteção da infraestrutura física global, hardware, softwares base, redes e a camada de virtualização que sustenta os serviços.
> 
> 💻 **Segurança NA Nuvem (Responsabilidade do Cliente):** Proteção e criptografia dos dados armazenados, gerenciamento de acessos (IAM), configurações de firewall/rede e aplicação de patches de Sistema Operacional (ex: em instâncias EC2).
---
*💡 Dica de Prova: Para alta disponibilidade, as aplicações devem ser distribuídas em múltiplas AZs dentro de uma mesma Região. Lembre-se de que o faturamento cessa imediatamente ao interromper ou deletar os recursos sob demanda.*
