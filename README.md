

# Benefícios do Azure

## Alta disponibilidade
O Azure foi projetado para oferecer disponibilidade global, com data centers distribuídos em diversas regiões. Isso significa que suas aplicações e serviços podem ser acessados a qualquer hora e lugar, reduzindo riscos de indisponibilidade. A arquitetura em múltiplas zonas e regiões garante que falhas locais não comprometam a continuidade do negócio.

## Escalabilidade
Com o Azure, você pode aumentar a capacidade de processamento, memória ou armazenamento de forma simples e rápida, sempre que a demanda do sistema crescer. Esse recurso permite que aplicações acompanhem o ritmo do negócio sem precisar de grandes investimentos em infraestrutura física.

## Elasticidade
Além de escalar, o Azure ajusta automaticamente os recursos provisionados de acordo com o uso em tempo real. Isso evita desperdício em momentos de baixa demanda e assegura desempenho consistente em períodos de pico. A elasticidade é essencial para empresas com cargas de trabalho variáveis.

## Confiabilidade
A plataforma foi construída para ser resiliente, oferecendo replicação de dados e mecanismos de failover automáticos. Isso garante que, mesmo em casos de falhas de hardware ou problemas regionais, os serviços continuem funcionando com mínima interrupção, aumentando a confiança dos usuários.

## Previsibilidade
O Azure fornece ferramentas avançadas de monitoramento e relatórios que permitem prever consumo e custos com precisão. Modelos de preços flexíveis possibilitam planejar investimentos de acordo com a necessidade real, evitando surpresas no orçamento e melhorando a gestão financeira da TI.

## Segurança
A segurança é prioridade no Azure, que adota padrões internacionais de conformidade, criptografia em repouso e em trânsito, além de monitoramento contínuo contra ameaças. Os clientes têm acesso a controles granulares de identidade e acesso, garantindo proteção robusta de dados e aplicações.

## Governança
Com o Azure, é possível implementar políticas de conformidade, definir restrições de uso e monitorar recursos em toda a organização. Isso garante que os ambientes estejam em conformidade com requisitos internos e regulatórios, além de reduzir riscos de uso indevido da infraestrutura.

## Gerenciabilidade
O gerenciamento no Azure é simplificado por meio do portal web, APIs e ferramentas de automação como o Azure CLI e o PowerShell. Isso permite aos administradores controlar, monitorar e otimizar recursos com eficiência, além de integrar processos de DevOps para maior agilidade e produtividade.


# Armazenamento no Azure

O Azure oferece diferentes opções de armazenamento em nuvem para atender desde aplicações simples até sistemas críticos que demandam alta disponibilidade e resiliência. Cada modelo de replicação possui características próprias de redundância, custo e confiabilidade, permitindo que empresas escolham a solução mais adequada conforme suas necessidades de negócio.  

## LRS (Locally Redundant Storage)
O LRS mantém **três cópias dos dados dentro de um único datacenter**. Ele garante proteção contra falhas locais de hardware, mas não protege contra indisponibilidade causada por problemas no datacenter inteiro. É a opção mais econômica e recomendada para dados não críticos ou que podem ser restaurados de outra fonte.

## GRS (Geo-Redundant Storage)
O GRS replica os dados de forma assíncrona para uma **região secundária geograficamente distante** da região primária. Assim, em caso de falha regional grave, os dados podem ser recuperados na região de backup. Ele oferece alta durabilidade e é ideal para **backup de longo prazo** e cenários de recuperação de desastres.

## ZRS (Zone-Redundant Storage)
O ZRS mantém **cópias sincronizadas dos dados em três zonas de disponibilidade diferentes** dentro da mesma região. Isso garante **alta disponibilidade e baixa latência**, já que a replicação ocorre localmente. É indicado para aplicações que precisam permanecer ativas mesmo em caso de falha em uma zona específica.

## GZRS (Geo-Zone-Redundant Storage)
O GZRS combina as vantagens do ZRS e do GRS. Ele mantém os dados replicados em **múltiplas zonas de uma região primária** e também em uma **região secundária geograficamente distante**. É a opção mais robusta e indicada para dados **extremamente críticos**, que exigem o máximo de resiliência contra falhas regionais e zoneais.

# Comparativo de Armazenamento no Azure

| Tipo  | Local de Replicação | Nível de Redundância | Custo | Cenário Ideal |
|-------|---------------------|----------------------|-------|---------------|
| **LRS** (Locally Redundant Storage) | 3 cópias em um único datacenter | Redundância local | Baixo | Dados que podem ser restaurados manualmente ou têm menor criticidade |
| **GRS** (Geo-Redundant Storage) | Região primária + região secundária distante | Alta redundância geográfica | Médio | Backup de longo prazo e proteção contra falhas regionais |
| **ZRS** (Zone-Redundant Storage) | 3 zonas de disponibilidade na mesma região | Alta disponibilidade regional | Médio | Aplicações que exigem baixa latência e alta disponibilidade local |
| **GZRS** (Geo-Zone-Redundant Storage) | Zonas de uma região + réplica em outra região | Máxima redundância (zonas + geográfica) | Alto | Dados críticos que precisam de resiliência total contra falhas regionais |
