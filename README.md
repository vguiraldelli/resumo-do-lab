# Microsoft AZ900 - DIO
Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO

## Resumo:
Até o momento foram apresentados apenas conceitos introdutórios sobre a Cloud da Azure voltada para IA.
Foi explicado sobre os tipos de Cloud, privada, híbrida ou pública, onde as empresas podem optar na utilização de nuvem privada, mantendo os dados isolados em ambientes On-Premises, híbrida, conectado os ambientes On-Premises a recursos de Cloud pública, ou simplesmente utilizar a Cloud pública se beneficiando em não precisar se preocupar com os gastos e energia de trabalho direcionadas para manter ambientes físicos e garantir a segurança dos dados, em vista que tudo isso já é oferecido na Cloud pública.
Em seguida, foi apresentado o Portal Azure, onde as ferramentas são organizadas em Categorias desde IA, Infraestrutura, etc...

O desafio da aula "Criando máquinas Virtuais na Azure" não esta claro, em uma aula anterior já foi feito o mesmo, mas estava explícito o que se esperava do desafio.

## Configurando uma instância de Banco de Dados na Azure
É preciso definir um servidor para a instância do Banco de Dados, isso possibilita escolher a melhor localidade para a disponibilidade da base de dados.
Se atentar para as configurações de Acessos e SLA.

## Computação e rede - Laboratório
Nesta aula foi apresentado como é criada uma máquina virtual (servidor ou máquina de trabalho) na núvem da Azure.
Atualmente a Microsoft já oferece padrões recomendados de máquina com configrações pré-definidas, o que pode agilizar a criação da máquina virtual.
É importante entender as diferentes necessidades de acordo com cada tipo de ambiente, como desenvolvimento, teste e produção, entre outras possibilidades.
Foi apresentada toda a trilha de criação de uma máquina virtual através dpo Portal Azure.

## Aula: Dominando o armazenamento do Azure
### Conta de Armazenamento
- Uma conta de armazenamento recebe dados de diversos tipos
- O nome da conta deve ser exclusivo globalmente e conter de 3 a 24 caracteres.

### Compartilhamento de arquivos
- Uma unidade de arquivos pode ser utilizada conectando-se a ela através de conexão SMB na porta 445.

### Migrações para Azure
Podemos migrar diferentes tipos de itens pra a Azure, sendo eles:
- Servidores, bancos de dados e aplicativos web.
- Banco de dados (somente)
- Aplicativos Web
- Data Box

No Data Box, temos algumas opções para solicitação:
- Data Box Disk: 35 TB
- Data Box: 80 TB
- Data Box Heavy: 800 TB

Ferramentas para migração:
- AzCopy: Uma ferramenta para copiar dados para nuvem de uma forma parecida com FTP. Funciona em Windows, Linux e MacOS.
- Gerenciador de Armazenamento do Microsoft Azure: Uma interface para acessar o conteúdo de contas de armazenamento e utilizar o AzCopy através da interface.

## Aula: Segurança e identidade no Azure

### Identidade:
- Microsoft Entra ID: Gerenciamento de usuários e acessos, com possibilidade de replicação dos usuários originados no AD Local para a Nuvem.
- Usuários deletados são removidos permanentemente depois de 30 dias.
- É possível fazer invites em lote via CSV.

### Defender for Cloud:
- É uma aplicação Cloud Native para gerenciar a segurança e integridade de ambientes.
- Compatível com Azure, AWS e GCP.
- Possui módulos de proteção para DevOps.

## Aula: Gerenciamento de Custos no Azure

### Calculadora do TCO (Custo Total de Propriedade):
- Link: (Calculadora TCO não encontrada)
- A calculadora do TCO serve para analisar e comparar o gasto com infraestrutura local em relação a Azure.

### Calculadora de Recursos
- [Calculadora de Recursos Azure](https://azure.microsoft.com/pt-br/pricing/calculator/ "https://azure.microsoft.com/pt-br/pricing/calculator/")
- Serve para calcular os custos estimados por hora ou mensais para usar o Azure.

## Aula: Gerenciando Políticas em Acessos Azure

### Governança e Conformidade:
- Azure Policys ajudam a impor padrões organizacionais e garantir a conformidade.
- Bloqueios de recursos são herdados por seus recursos filhos. Os dois tipos de bloqueio são: Excluir e ReadOnly.
- [Portal de confiança do Serviço:](https://servicetrust.microsoft.com "https://servicetrust.microsoft.com") Serve para verificar quais protocolos, regras e padrões a Microsoft aplica.
- Microsoft Pureview: Uma ferramenta para governança para gerenciar os riscos e conformidade de dados tanto locais, multinuvem e SaS.

## Aula: Ferramentas de Gerenciamento e Implantação na Azure

### Ferramentas:
- A implantação de recursos na Azure pode ser feita inteiramente via Portal Azure, mas em algum momento surge a necessidade de implementar uma arquitetura em escala, onde se torna inviável a implantação via Portal.
A Azure fornece modelos de Scripts de implementação no Portal, podendo ser alterados e reutilizados em escala.
- ARM: É uma camada responsável por gerenciar as solicitações de implementação de recursos na Azure. É quem recebe e interpreta as solicitações.
- ARC: É uma ferramenta de gerenciamento Multi-Cloud
