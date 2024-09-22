# Rusumo dos laboratórios

## Computação em nuvem
Durante o laboratório, foi apresentado o Microsoft Azure e suas possibilidades de aplicação, então busquei aprender mais sobre alguns dos temas mencionados.

Começando pelos Bastions e Jump Servers, aprendi que eles são componentes essenciais para acessar recursos privados em uma rede segura. O Bastion atua como uma ponte, permitindo o acesso remoto a máquinas virtuais sem a necessidade de expor portas RDP ou SSH diretamente à internet, aumentando a segurança. Já o Jump Server funciona de maneira similar, servindo como um ponto centralizado de acesso aos servidores em uma rede restrita. Ambos garantem que o acesso aos recursos na nuvem seja mais seguro, evitando brechas de segurança que poderiam ser exploradas se os servidores estivessem expostos publicamente.

Quanto aos Firewalls na nuvem, entendi que eles são fundamentais para controlar e proteger o tráfego de rede. Eles agem como uma barreira entre diferentes zonas da rede, permitindo que o tráfego autorizado entre e saia, ao mesmo tempo que bloqueiam acessos não autorizados. Na nuvem, o firewall se torna ainda mais crucial, uma vez que os recursos estão distribuídos em múltiplas localizações e acessíveis de qualquer lugar do mundo.

Por fim, o armazenamento na nuvem foi outro conceito que explorei. Ele oferece alta disponibilidade, escalabilidade e redundância, permitindo o armazenamento de grandes quantidades de dados de forma segura e acessível. Soluções como o Blob Storage no Azure facilitam o armazenamento de arquivos e objetos na nuvem, além de permitir o acesso via API para integração com outros sistemas. No entanto, é necessário que uma empresa analise a viabilidade de usar o armazenamento na nuvem.

## Benefícios da nuvem - Azure
O Azure oferece um serviço que pode ser personalizado de acordo com a sua demanda.

| SLA       | Tempo de inatividade por semana | Tempo de inatividade por mês | Tempo de inatividade por ano |
|-----------|---------------------------------|------------------------------|------------------------------|
| 99%       | 1,68 hora                       | 7,2 horas                    | 3,65 dias                    |
| 99,9%     | 10,1 minutos                    | 43,2 minutos                 | 8,76 horas                   |
| 99,95%    | 5 minutos                       | 21,6 minutos                 | 4,38 horas                   |
| 99,99%    | 1,01 minuto                     | 4,32 minutos                 | 52,56 minutos                |
| 99,999%   | 6 segundos                      | 25,9 segundos                | 5,26 minutos                 |

Fonte: [Azure Well-Architected Framework - Métricas de Confiabilidade](https://learn.microsoft.com/pt-br/azure/well-architected/reliability/metrics)

Antes de realizar a contratação de um serviço como esse, é sempre importante saber qual nível de criticidade é necessario para a sua aplicação, para que o resultado seja mais satisfatorio. O tempo de inatividade não pode ser um impeditivo para que sua aplicação funcione no momento certo.

As máquinas virtuais no Azure são um dos serviços essenciais oferecidos pela plataforma de computação em nuvem da Microsoft. Elas permitem a criação e execução de instâncias de máquinas virtuais personalizáveis na infraestrutura em nuvem do Azure, de forma semelhante a servidores físicos. 

O Azure oferece opções de alta disponibilidade, como zonas de disponibilidade, que garantem que o serviço continue funcionando mesmo em caso de falhas de hardware ou em data centers.

## Tipos de serviço de nuvem
Uma imagem de máquina virtual (VM) no Azure é uma cópia pré-configurada de um sistema operacional, que pode incluir software e configurações específicas. As imagens são usadas para criar novas instâncias de máquinas virtuais rapidamente e de forma consistente. O Azure fornece uma variedade de imagens padrão que incluem diferentes sistemas operacionais, como Windows Server, Ubuntu, e outras distribuições Linux.

Os bancos de dados no Azure são serviços de armazenamento de dados que permitem gerenciar, consultar e armazenar informações de forma eficiente. O Azure oferece várias opções de banco de dados, como MySQL, PostgreSQL, MariaDB, etc. Bancos de dados na nuvem podem ser facilmente escalados para atender a demandas variáveis, aumentando ou diminuindo recursos de acordo com a necessidade. Eles também podem ser acessados de qualquer lugar com conexão à internet, facilitando o trabalho remoto e a colaboração. Além disso, tanto a Azure como outros provedores de nuvem, cuidam de tarefas administrativas, como backups, atualizações de software e patches de segurança, permitindo que os desenvolvedores se concentrem na construção de aplicativos.
