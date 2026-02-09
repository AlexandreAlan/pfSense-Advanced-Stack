# 📊 Traffic Shaping & Bandwidth Control

Nesta seção, exploramos as duas principais metodologias de gerenciamento de tráfego no pfSense. A escolha entre uma ou outra depende do objetivo: controle estrito de banda ou priorização inteligente de serviços.

## 🗂️ Estrutura do Módulo

O conteúdo está dividido em duas abordagens distintas:

### 1. [Limiters (Dummynet)](./Limiters/)
Focado no controle de largura de banda (Download/Upload) por host ou rede. É a solução ideal para:
* Limitar a velocidade de redes de Visitantes/Guest.
* Mitigar o *Bufferbloat* utilizando o algoritmo **FQ_CODEL**.
* Garantir que nenhum usuário consuma todo o link sozinho.

### 2. [QoS & ALTQ Shaper](./QoS-ALTQ/)
Focado na priorização de protocolos e baixa latência para serviços críticos. Ideal para:
* Priorizar tráfego de **VoIP** e reuniões (Teams/Meet).
* Garantir que o tráfego de DNS e ACKs passe na frente de downloads.
* Gerenciamento de filas baseadas em prioridade (HFSC, CBQ ou PRIQ).

---

## 🚀 Qual utilizar?
No dia a dia corporativo, a combinação de ambos ou o uso estratégico de Limiters modernos (2.7.2+) costuma entregar o melhor resultado para links de alta velocidade. 

*Consulte os READMEs dentro de cada pasta para o guia de configuração passo a passo.*
