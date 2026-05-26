# Fundamentos da Nuvem e Infraestrutura Global

Este resumo aborda os conceitos iniciais sobre como a infraestrutura global da AWS está organizada e como o modelo de computação impacta o desenvolvimento de aplicações.

## 🏢 Infraestrutura Global
* **Regiões (Regions):** Locais geográficos distintos ao redor do mundo que hospedam clusters de data centers. Elas são completamente isoladas umas das cores para garantir a máxima tolerância a falhas e estabilidade.
* **Zonas de Disponibilidade (AZs - Availability Zones):** Um ou mais data centers discretos com energia, rede e conectividade redundantes dentro de uma Região AWS. Elas são conectadas por redes de latência ultrabaixa.

## 💰 Modelo de Faturamento
* **Pay-as-you-go (Pagamento por uso):** Modelo de precificação sob demanda onde você paga apenas pelos recursos computacionais que consome, sem a necessidade de investimentos iniciais pesados ou contratos de longo prazo. Permite escalar custos linearmente com o uso.

---
*💡 Dica de Prova: Para alta disponibilidade, as aplicações devem ser distribuídas em múltiplas AZs dentro de uma mesma Região. Lembre-se de que o faturamento cessa imediatamente ao interromper ou deletar os recursos sob demanda.*
