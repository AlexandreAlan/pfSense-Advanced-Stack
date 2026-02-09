# pfSense-Advanced-Stack
Seja bem-vindo ao pfSense Advanced Stack. Este repositório não é apenas um guia de comandos, mas um framework completo de endurecimento (hardening) e otimização de borda para ambientes corporativos que exigem o máximo de controle, auditoria e performance.

Neste projeto, detalho a implementação de arquiteturas complexas utilizando o pfSense como core de rede, abordando:
🛠️ Core Engineering & Traffic Management

    Traffic Shaping de Próxima Geração: Implementação de Limiters utilizando algoritmos FQ_CODEL e Tail Drop para mitigação de Bufferbloat, garantindo latência submilisegundo para serviços críticos (VoIP, Videoconferência) mesmo sob saturação de link.

    WPAD & Proxy Auto-Discovery: Configuração de descoberta automática via DNS (opção 252) e DHCP, integrando scripts wpad.dat e proxy.pac para roteamento inteligente de tráfego web sem intervenção manual no host.

🔐 Identity & Access Management (IAM)

    Captive Portal Multi-Tier: Arquitetura de portal personalizado em PHP com backend de autenticação via FreeRADIUS integrado a um banco de dados MySQL Externo. Suporte a auto-cadastro, controle de sessão simultânea e persistência de dados.

    Segurança de Gerenciamento: Hardening da interface WebGUI via HTTPS com certificados SSL/TLS, alteração de portas padrão, desativação de contas genéricas e implementação de privilégios granulares para usuários administrativos (Role-Based Access Control).

🛡️ Advanced Security & Filtering

    DNSBL & Blacklisting Granular: Orquestração de listas de bloqueio personalizadas via pfBlockerNG, com foco em telemetria, prevenção de intrusão (IP de reputação ruim) e filtragem de conteúdo por categoria (Adulto, Apostas, Criptomineradores).

    Firewall State Optimization: Ajustes finos na tabela de estados para ambientes de alta densidade, otimizando o consumo de memória e CPU do hardware.

⚖️ Compliance e Governança

    Conformidade LGPD: Estruturação de logs de acesso e políticas de monitoramento de rede, garantindo que a coleta de dados de navegação esteja devidamente documentada e protegida, respeitando a privacidade e os requisitos legais brasileiros.

Por que este repositório é diferente?

Diferente de tutoriais básicos, aqui focamos em escalabilidade. Todas as soluções propostas são testadas em cenários de alta carga, visando eliminar gargalos de hardware e garantir que o firewall não seja o ponto único de falha da rede.
