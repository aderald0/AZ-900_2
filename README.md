# AZ-900_2
Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO

Microsoft Azure oferece uma ampla gama de serviços em nuvem, organizados em várias categorias para facilitar a localização e o uso. Aqui está um resumo das principais categorias de serviços no Azure:

Computação: Oferece serviços como Máquinas Virtuais (VMs), App Services, e Azure Kubernetes Service (AKS), permitindo escalabilidade e execução de aplicativos.

Rede: Inclui serviços como Azure Virtual Network, Load Balancer, VPN Gateway, para conectar e gerenciar redes virtuais de maneira segura e eficiente.

Armazenamento: Soluções para armazenamento de dados, como Blob Storage, File Storage, e Disk Storage, adaptados para diferentes necessidades de desempenho e redundância.

Bancos de Dados: Oferece bancos de dados gerenciados, como Azure SQL Database, Cosmos DB (NoSQL), e Azure Database for MySQL/PostgreSQL, com alta disponibilidade e escalabilidade.

Inteligência Artificial e Machine Learning: Serviços como Azure Cognitive Services, Azure Machine Learning, e Bot Services para implementar IA e aprendizado de máquina em soluções empresariais.

DevOps: Serviços como Azure DevOps e Azure Pipelines para integração contínua (CI) e entrega contínua (CD), além de ferramentas para gerenciar o ciclo de vida de aplicativos.

Identidade e Segurança: Serviços como Azure Active Directory (AAD) e Azure Security Center, que ajudam a proteger recursos e gerenciar identidades de usuários e acessos.

Monitoramento e Gerenciamento: Inclui serviços como Azure Monitor, Azure Policy, e Log Analytics, que fornecem visibilidade sobre a integridade e o desempenho dos aplicativos e infraestrutura.

IoT: Oferece serviços como Azure IoT Hub e Azure Digital Twins para soluções de Internet das Coisas (IoT), permitindo a conexão e gestão de dispositivos.

Análise e Big Data: Soluções como Azure Synapse Analytics, HDInsight, e Data Lake Storage para gerenciamento e análise de grandes volumes de dados.

Essas categorias facilitam a busca e a seleção de serviços conforme as necessidades específicas de infraestrutura, desenvolvimento ou segurança em projetos de TI na nuvem.






Você disse:
Criando máquinas Virtuais na Azure faça um resumo
O ChatGPT disse:
ChatGPT
Criar Máquinas Virtuais (VMs) no Microsoft Azure é uma maneira eficaz de rodar aplicativos ou hospedar serviços na nuvem, com flexibilidade e escalabilidade. Aqui está um resumo do processo de criação de VMs no Azure:

1. Acesso ao Portal Azure
Acesse o Portal Azure (portal.azure.com) com uma conta ativa.
2. Início da Criação da Máquina Virtual
No painel do portal, clique em "Criar um recurso".
Selecione a categoria "Máquinas Virtuais".
3. Configuração Básica da VM
Escolha o grupo de recursos onde a VM será criada (ou crie um novo).
Defina o nome da VM, a região onde ela será hospedada e a imagem do sistema operacional (Windows, Linux).
Selecione o tamanho da VM com base em vCPU, RAM e necessidades de desempenho.
4. Autenticação e Rede
Configure o método de autenticação: chave SSH (para Linux) ou senha (para Windows).
Defina as configurações de rede: Rede Virtual, Sub-rede, e escolha se a VM terá um endereço IP público.
5. Configurações de Armazenamento
Escolha o tipo de disco (SSD ou HDD) e configure o armazenamento adicional conforme necessário.
6. Revisar e Criar
Revise todas as configurações e clique em "Criar" para provisionar a VM.
7. Gerenciamento da VM
Após a criação, é possível acessar a VM pelo Portal Azure, ou via SSH (Linux) ou RDP (Windows).
Utilize o Azure Monitor para acompanhar o desempenho, escalabilidade, e a integridade da VM.
Benefícios
Escalabilidade: Fácil aumento ou redução dos recursos conforme necessário.
Automação: Pode-se usar scripts e templates do Azure Resource Manager (ARM) para automação.
Integração: As VMs podem ser integradas a outros serviços, como redes virtuais, balanceadores de carga e firewalls.
Esse processo oferece flexibilidade na escolha de sistemas operacionais e configurações, garantindo uma solução sob medida para qualquer aplicação ou serviço que você deseja executar na nuvem.






Você disse:
sla azure
O ChatGPT disse:
ChatGPT
O SLA (Service Level Agreement) no Microsoft Azure define o nível de disponibilidade e confiabilidade garantido para os diversos serviços oferecidos na plataforma. Ele estabelece os compromissos de tempo de atividade (uptime) que a Microsoft oferece para garantir a operação contínua dos serviços. Aqui está um resumo dos principais pontos sobre o SLA no Azure:

1. Níveis de Disponibilidade (Uptime)
O Azure garante altos níveis de disponibilidade para seus serviços, variando conforme o tipo de recurso. Alguns exemplos:

Máquinas Virtuais (VMs): Até 99,99% de disponibilidade quando configuradas em Conjuntos de Disponibilidade (Availability Sets) ou Zonas de Disponibilidade (Availability Zones).
Armazenamento: 99,9% de tempo de atividade garantido para Azure Storage.
Bancos de Dados Gerenciados: 99,99% de disponibilidade para serviços como Azure SQL Database e Cosmos DB.
2. Zonas de Disponibilidade e Conjuntos de Disponibilidade
Utilizar Zonas de Disponibilidade (em regiões que oferecem essa funcionalidade) garante maior resiliência, com disponibilidade de até 99,99%.
Máquinas virtuais distribuídas em Conjuntos de Disponibilidade garantem proteção contra falhas de hardware em um único datacenter.
3. Redundância e Resiliência
O Azure oferece diferentes níveis de redundância, como cópias de dados georredundantes, para garantir que os serviços possam se recuperar de falhas ou desastres.
4. Créditos por Quebra de SLA
Se o Azure não atingir o nível de serviço garantido (disponibilidade menor do que o especificado no SLA), o cliente pode ser elegível para créditos financeiros na sua assinatura. Esses créditos variam conforme o nível de indisponibilidade e o serviço afetado.
5. Monitoramento e Manutenção
O SLA cobre apenas períodos fora de janelas de manutenção programada. O Azure pode executar atualizações ou manutenções em determinados serviços, o que pode afetar a disponibilidade temporariamente, mas esses períodos são excluídos do cálculo de SLA.
6. Responsabilidades do Usuário
Para atingir as garantias de SLA, muitas vezes é necessário que os usuários configurem adequadamente os serviços, como usar VMs em Availability Sets ou Zonas de Disponibilidade, habilitar backups e monitoramento.
Exemplo de SLA
Máquinas Virtuais com Disco Gerenciado:
99,9% de disponibilidade para uma única instância de VM.
99,99% de disponibilidade para VMs distribuídas em Availability Zones.
O SLA do Azure fornece uma base para garantir a continuidade dos serviços e mitigar impactos em caso de falhas, sendo fundamental para empresas que dependem de alta disponibilidade e resiliência em suas operações.
