# AWS Academy Cloud Foundation (Fundamentos de nuvem do AWS Academy)

<div>
    <img alt="Criado por Alcir Junior [Caju]" src="https://img.shields.io/badge/criado%20por-Alcir Junior [Caju]-%23f08700">
    <img alt="License" src="https://img.shields.io/badge/license-MIT-%23f08700">
</div>

---

## Descrição

Curso oferecido pelo **Centro de Desenvolvimento e Formação Continuada em Informática Biomédica (CDFC - IBm/FMRP)**, em conjunto com a **AWS Academy**. Destinado a estudantes que buscam compreender os conceitos de computação em nuvem, independentemente de funções técnicas específicas. O curso provê uma visão geral detalhada dos conceitos de nuvem, principais serviços AWS, segurança, arquitetura, definição de preço e suporte.

---

## Visualizar o projeto na IDE:

Para quem quiser visualizar o projeto na IDE clique no teclado a tecla `ponto`, esse recurso do GitHub é bem bacana

---

# Módulo 3: Visão Geral da Infraestrutura Global da AWS

### Boas-vindas e Introdução
Introdução à forma como a AWS organiza sua infraestrutura massiva ao redor do mundo.

---

### Tópicos Abordados
* **Infraestrutura Global da AWS:** Como a AWS está fisicamente distribuída.
* **Visão Geral dos Serviços e Categorias:** Conhecer os diferentes tipos de serviços que a AWS oferece.

---

### Recursos de Aprendizagem Disponíveis
Para aprofundar seu conhecimento, você terá acesso a:
* **Demonstração:** Focada nos detalhes da Infraestrutura Global.
* **Atividade Prática (Hands-on):** Oportunidade para explorar o Console de Gerenciamento da AWS.
* **Verificação de Conhecimento:** Um teste para avaliar sua compreensão dos conceitos-chave.

---

### Objetivos de Aprendizagem
Ao final deste módulo, você será capaz de:
* Diferenciar claramente os conceitos de:
    * **Regiões da AWS**
    * **Zonas de Disponibilidade (Availability Zones)**
    * **Locais de Borda (Edge Locations)**
* Identificar os principais serviços e suas respectivas categorias na AWS.

# Visão Geral dos Serviços e Categorias de Serviços da AWS

## Introdução

A AWS oferece um amplo conjunto de produtos globais baseados em nuvem que podem ser usados como blocos de construção para arquiteturas de nuvem comuns.

### A Plataforma AWS

A infraestrutura global da AWS pode ser dividida em três elementos:

#### Regiões
* Uma **Região AWS** é uma área geográfica.
    * A **replicação de dados** entre Regiões é controlada por você.
    * A **comunicação** entre regiões usa a infraestrutura de rede backbone da AWS.
* Cada região fornece redundância total e conectividade com a rede.
* Uma Região normalmente consiste em duas ou mais **Zonas de Disponibilidade**.

A infraestrutura da Nuvem AWS é criada em torno das regiões. A AWS tem 22 Regiões em todo o mundo. Uma **Região AWS** é uma localização geográfica física com uma ou mais **Zonas de Disponibilidade**. As Zonas de Disponibilidade, por sua vez, consistem em um ou mais **data centers**.

Para alcançar tolerância a falhas e estabilidade, as regiões são isoladas umas das outras. Os recursos em uma região não são replicados automaticamente para outras regiões. Quando você armazena dados em uma região específica, eles não são replicados fora dessa região.

É sua responsabilidade replicar dados entre regiões, caso suas necessidades empresariais exijam isso.

As Regiões AWS que foram introduzidas antes de 20 de março de 2019 são ativadas por padrão. As Regiões que foram introduzidas após 20 de marçode 2019, como Ásia-Pacífico (Hong Kong) e Oriente Médio (Bahrein), são desativadas por padrão. É necessário ativar essas Regiões para que você possa usá-las. Você pode usar o Console de Gerenciamento da AWS para habilitar ou desabilitar uma região.

Algumas regiões têm acesso restrito. Uma conta da Amazon AWS (China) fornece acesso somente às Regiões de Pequim e Ningxia. Para saber mais sobre a AWS na China, consulte: https://www.amazonaws.cn/en/about-aws/china/.

A região isolada AWS GovCloud (EUA) foi projetada para permitir que clientes e órgãos governamentais dos EUA transfiram cargas de trabalho confidenciais para a nuvem, cumprindo seus requisitos normativos e de conformidade específicos.

Há alguns fatores que você deve considerar ao selecionar a Região ou Regiões ideais onde você armazena dados e usa os serviços da AWS.

Uma consideração essencial é a governança de dados e os requisitos legais. As leis locais podem exigir que determinadas informações sejam mantidas dentro de limites geográficos. Essas leis podem restringir as Regiões onde é possível oferecer conteúdo ou serviços. Por exemplo, considerea Diretiva de Proteção de Dados da União Europeia(UE).

Se todos os demais fatores permanecem iguais, de modo geral é desejável executar suas aplicações e armazenar seus dados em uma Região que esteja mais próxima possível do usuário e dos sistemas que os acessarão. Isso ajudará você areduzir a latência. O CloudPing é um site que pode ser usado para testar a latência entre sua localização e em todas as Regiões AWS. Para saber mais sobre o CloudPing, consulte: https://www.cloudping.info

Por fim, há alguma variação no custo da execução de serviços, que pode depender da Região escolhida. Por exemplo, no momento em este texto foi escrito, a execução de uma instância Linux do Amazon Elastic Compute Cloud (Amazon EC2) t3.medium sob demanda na Região Leste dos EUA (Ohio) custa 0,0416 USD por hora, mas a execução da mesma instância na Região Ásia-Pacífico (Tóquio) custa 0,0544 USD por hora.

#### Zonas de disponibilidade
* Cada **Região** tem várias Zonas de Disponibilidade.
* Cada **Zona de Disponibilidade** é uma partição totalmente isolada da infraestrutura da AWS.
    * As Zonas de Disponibilidade consistem em **data centers** distintos
    * Elas são projetadas para isolamento de falhas
    * Elas são interconectadas a outras zonas de disponibilidade usando redes privadas de alta velocidade
    * Você escolhe suas zonas de disponibilidade
    * **A AWS recomenda a replicação de dados e recursos entre Zonas de Disponibilidade** para fins de resiliência

Cada Região AWS contém vários locais isolados, conhecidos como Zonas de Disponibilidade.

Cada Zona de Disponibilidade oferece a capacidade de operar aplicativos e bancos de dados mais altamente disponíveis, tolerantes a falhas e dimensionáveis do que seria possível em um único data center. Cada Zona de Disponibilidade pode incluir vários data centers (normalmente três) e, em dimensão integral, eles podem incluir centenas de milhares de servidores. Elas são partições totalmente isoladas da infraestrutura global da AWS. As Zonas de Disponibilidade têm sua própria infraestrutura de energia e são fisicamente separadas por muitos quilômetros de outras Zonas de Disponibilidade, embora todas elas estejam a 100 km umas das outras.

Todas as Zonas de Disponibilidade são interconectadas com redes de alta largura de banda e baixa latência por meio de fibra dedicada totalmente redundante que fornece alta vazão entre as Zonas de Disponibilidade. A rede faz a replicação síncrona entre as Zonas de Disponibilidade.

As Zonas de Disponibilidade ajudam a criar aplicativos altamente disponíveis. Quando uma aplicação é particionada entre Zonas de Disponibilidade, as empresas estarão melhor isoladas e protegidas contra problemas como relâmpagos, tornados, terremotos, entre outros.

Você é responsável por escolher as Zonas de Disponibilidade em que os sistemas serão armazenados. Os sistemas podem abranger várias Zonas de Disponibilidade. A AWS recomenda a replicação entre zonas de disponibilidade para fins de resiliência. Você deve projetar os sistemas para sobreviverem a uma falha temporária ou prolongada de uma zona de disponibilidade se ocorrer um desastre.

#### Data centers da AWS
* Os data centers da AWS são projetados para segurança.
* Os data centers são onde os dados residem e o processamento de dados ocorre.
* Cada data center tem energia, redes e conectividade redundantes e está hospedado em uma instalação separada.
* Normalmente, um data center tem de 50.000 a 80.000 servidores físicos.

A base da infraestrutura da AWS são os data centers. Os clientes não especificam um data center para a implantação de recursos. Em vez disso, uma Zona de Disponibilidade é o nível de especificação mais granular que um cliente pode fazer. No entanto, um data center é o local onde os dados reais residem. A Amazon opera data centers de última geração e altamente disponíveis. Embora sejam raras, podem ocorrer falhas que afetam a disponibilidade das instâncias no mesmo local. Se você hospedar todas as suas instâncias em um único local afetado por essa falha, nenhuma delas estará disponível.

Os data centers são projetados com segurança, com vários fatores em mente:

Cada local é cuidadosamente avaliado para **mitigar os riscos do ambiente**.
* Os data centers têm um **design redundante** que prevê e tolera falhas enquanto mantém os níveis de serviço.
* Para garantir a disponibilidade, **o backup de componentes críticos do sistema** é feito em várias Zonas de Disponibilidade.
* A AWS monitora continuamente o uso dos serviços para implantar uma infraestrutura que ofereça suporte aos nossos compromissos e requisitos de disponibilidade.
* Data centers: **seus locais não são divulgados** e todo o acesso a eles é restrito.
* Em caso de falha, processos automatizados desviam o tráfego de dados da área afetada.

A AWS usa **equipamentos de rede personalizados** de **vários fabricantes de dispositivos originais (ODMs)**. Os ODMs projetam e fabricam produtos com base nas especificações de uma segunda empresa. Esta então cria uma nova marca para os produtos e os revende.

#### Pontos de presença (que incluem os locais de borda)
* A AWS fornece uma rede global de locais de **pontos de presença**
* Consiste em **locais de borda** e um número muito menor de **caches de borda regionais**
* Usada com o Amazon CloudFront
    * Uma Content Delivery Network (CDN - Rede de entrega de conteúdo) global que entrega conteúdo aos usuários finais **comlatência reduzida**
* Os pontos de presença de caches regionais usados para conteúdo com acesso pouco frequente

**O Amazon CloudFront** é **uma rede de entrega de conteúdo (CDN)** usada para distribuir conteúdo aos usuários finais para reduzir a latência. O Amazon Route 53 é um serviço de sistema de nomes de domínio (DNS). As solicitações enviadas para qualquer um desses serviços serão roteadas automaticamente para o ponto de presença mais próximo para diminuir a latência.

Os **pontos de presença da AWS** estão localizados na maioria das principais cidades do mundo. Ao **medir continuamente a conectividade, o desempenho e a computação com a Internet para encontrar a melhor maneira de rotear solicitações**, os pontos de presença oferecem uma melhor experiência de usuário quase em tempo real. Eles são usados por muitos serviços da AWS, incluindo os serviços Amazon CloudFront, Amazon Route 53, AWS Shield e AWS Web Application Firewall (AWS WAF).

Os **caches de borda regionais** são usados com o Amazon CloudFront por padrão. Os caches de borda regionais são usados quando você tem conteúdo que não é acessado com frequência suficiente para permanecer em um **local de borda**. Os caches de borda regionais absorvem esse conteúdo e fornecem uma alternativa para obter esse conteúdo no servidor de origem.

Essa infraestrutura fornece a plataforma para um vasto conjunto de serviços, como redes, armazenamento, serviços de computação e bancos de dados.

Esses serviços são entregues como um utilitário sob demanda (on-demand), disponível em segundos, com preços no modelo pague-pelo-uso (pay-as-you-go).

### Recursos de infraestrutura da AWS
* Elasticidade e dimensionamento
    * Infraestrutura elástica; adaptação dinâmica da capacidade
    * Infraestrutura escalável; adapta-se para acomodar o crescimento
* Tolerância a falhas
    * Continua funcionando corretamente na presença de uma falha
    * Redundância integrada de componentes
* Alta disponibilidade
    * Alto nível de desempenho operacional
    * Tempo de inatividade mínimo
    * Sem intervenção humana

Agora que você tem uma boa compreensão dos principais componentes que compõem a infraestrutura global da AWS, vamos considerar os benefícios oferecidos por essa infraestrutura.

A infraestrutura global da AWS tem vários recursos valiosos:
* Primeiro, ela é elástica e dimensionável. Isso significa que os recursos podem se ajustar dinamicamente para aumentos ou diminuições nos requisitos de capacidade. Ele também pode se ajustar rapidamente para acomodar o crescimento.
* Em segundo lugar, essa infraestrutura é tolerante a falhas, o que significa que ela tem redundância de componentes integrada que permite continuar as operações apesar de falha em um componente.
* Por fim, ela requer intervenção mínima a nenhuma intervenção humana, enquanto fornece alta disponibilidade com tempo de inatividade mínimo.

### Conclusão
* A **infraestrutura global da AWS** consiste em **Regiões** e **Zonas de Disponibilidade**.
* Normalmente, a escolha de uma **Região** é baseada em **requisitos de conformidade** ou para **reduzir a latência**.
* Cada **Zona de Disponibilidade** é fisicamente separada de outras zonas de disponibilidade e tem alimentação, redes e conectividade redundantes.
* **Locais de borda** e **caches de borda regionais** melhoram o desempenho **armazenando conteúdo** em cache em locais mais próximos dos usuários.

### Foco do Curso

Existem 23 categorias diferentes de produtos ou serviços, e cada categoria consiste em um ou mais serviços. Este curso não tentará apresentar cada um deles. Em vez disso, o foco é nos serviços mais amplamente utilizados e que oferecem a melhor introdução à Nuvem AWS. O curso também se concentra nos serviços que têm maior probabilidade de serem abordados no exame AWS Certified Cloud Practitioner.

---

## Serviços de Armazenamento (Storage)

* **Amazon Simple Storage Service (Amazon S3):** É um serviço de armazenamento de objetos que oferece dimensionamento, disponibilidade de dados, segurança e desempenho. Use-o para armazenar e proteger qualquer quantidade de dados para sites, aplicativos móveis, backup e restauração, arquivo, aplicativos empresariais, dispositivos da Internet das Coisas (IoT) e análises de big data.
* **Amazon Elastic Block Store (Amazon EBS):** É um serviço de armazenamento em blocos de alto desempenho projetado para uso com o AmazonEC2 para cargas de trabalho com throughpute uso intensivo de transações. Ele é usado para várias cargas de trabalho, como bancos de dados relacionais e não relacionais, aplicativos empresariais, aplicativos em contêiner, mecanismos de análise de big data, sistemas de arquivos e fluxos de trabalho de mídia.
* **Amazon Elastic File System (Amazon EFS):** Fornece um sistema de arquivos NFS totalmente gerenciado, dimensionável e elástico para uso com os AWS Cloud Services e recursos on-premises. Ele foi desenvolvido para dimensionar sob demanda, aumentando e diminuindo automaticamente à medida que você adiciona e remove arquivos. Ele reduz a necessidade de provisionar e gerenciar capacidade para acomodar o crescimento.
* **Amazon S3 Glacier:** É uma classe de armazenamento na nuvem do AmazonS3 segura, durável e de custo extremamente baixo para arquivamento de dados e backup de longo prazo. Ele foi projetado para fornecer 11 noves de durabilidade e para fornecer recursos abrangentes de segurança e conformidade para cumprir requisitos normativos rigorosos.

---

## Serviços de Computação (Compute)

* **Amazon Elastic Compute Cloud (Amazon EC2):** Fornece capacidade de computação redimensionável como máquinas virtuais na nuvem.
* **Amazon EC2 Auto Scaling:** Permite adicionar ou remover automaticamente instâncias EC2 de acordo com as condições que você define.
* **Amazon Elastic Container Service (Amazon ECS):** Um serviço de orquestração de contêineres de alta performance e escalabilidade que suporta contêineres Docker.
* **Amazon Elastic Container Registry (Amazon ECR):** Um registro de contêineres Docker totalmente gerenciado que facilita para os desenvolvedores armazenar, gerenciar e implantar imagens de contêineres Docker.
* **AWS Elastic Beanstalk:** Um serviço para implantar e escalar aplicações e serviços web em servidores familiares, como Apache e Microsoft Internet Information Services (IIS).
* **AWS Lambda:** Permite que você execute código sem provisionar ou gerenciar servidores. Você paga apenas pelo tempo de computação que consome; não há cobrança quando seu código não está em execução.
* **Amazon Elastic Kubernetes Service (Amazon EKS):** Facilita a implantação, o gerenciamento e a escala de aplicações em contêineres que usam Kubernetes na AWS.
* **AWS Fargate:** Um mecanismo de computação para o Amazon ECS que permite executar contêineres sem ter que gerenciar servidores ou clusters.

---

## Serviços de Banco de Dados (Database)

* **Amazon Relational Database Service (Amazon RDS):** Um banco de dados relacional na nuvem fácil de configurar, operar e escalar. Fornece capacidade redimensionável enquanto automatiza tarefas administrativas demoradas.
* **Amazon Aurora:** Um banco de dados relacional compatível com MySQL e PostgreSQL. É configurado para ser cinco vezes mais rápido que os bancos de dados MySQL padrão e três vezes mais rápido que os bancos de dados PostgreSQL padrão.
* **Amazon Redshift:** Permite executar consultas analíticas em petabytes de dados armazenados localmente na Amazon. Oferece desempenho rápido em qualquer escala.
* **Amazon DynamoDB:** Um banco de dados NoSQL de chave-valor e de documentos totalmente gerenciado que oferece desempenho de milissegundos de um dígito em qualquer escala, com segurança integrada, backup e restauração, e cache em memória.

---

## Redes e Entrega de Conteúdo (Networking & Content Delivery)

* **Amazon Virtual Private Cloud (Amazon VPC):** Permite provisionar seções logicamente isoladas da Nuvem AWS para lançar recursos AWS em uma rede virtual que você define.
* **Elastic Load Balancing (ELB):** Distribui automaticamente o tráfego de entrada de aplicações entre múltiplos alvos, como instâncias Amazon EC2, contêineres, endereços IP e funções Lambda.
* **Amazon CloudFront:** Uma rede de entrega de conteúdo (CDN) rápida que entrega de forma segura dados, vídeos, aplicações e APIs a clientes globalmente com baixa latência e altas velocidades de transferência.
* **AWS Transit Gateway:** Permite que os clientes conectem suas Amazon VPCs e suas redes on-premises a um único gateway gerenciado centralmente.
* **Amazon Route 53:** Um serviço web de Sistema de Nomes de Domínio (DNS) em nuvem, escalável e projetado para oferecer uma maneira confiável de rotear usuários finais para aplicações na internet. Ele traduz URLs para os endereços IP numéricos que os computadores usam para se conectar.
* **AWS Direct Connect:** Fornece uma maneira de estabelecer uma conexão de rede privada dedicada do seu data center ou escritório para a AWS, o que pode reduzir custos e aumentar a largura de banda.
* **AWS VPN:** Fornece um túnel privado seguro da sua rede ou dispositivo para a Rede Global da AWS.

---

## Segurança, Identidade e Conformidade (Security, Identity & Compliance)

* **AWS Identity and Access Management (IAM):** Permite gerenciar o acesso aos serviços e recursos da AWS de forma segura.
* **AWS Organizations:** Permite restringir quais serviços e ações são permitidos em suas contas.
* **Amazon Cognito:** Permite adicionar autenticação de usuário e controle de acesso aos seus aplicativos web e móveis.
* **AWS Artifact:** Fornece acesso sob demanda a relatórios de segurança e conformidade da AWS, bem como a acordos online selecionados.
* **AWS Key Management Service (AWS KMS):** Permite criar e gerenciar chaves de criptografia para controlar o uso da criptografia em uma ampla gama de serviços AWS e em suas aplicações.
* **AWS Shield:** Um serviço gerenciado de proteção contra negação de serviço distribuída (DDoS) que protege as aplicações em execução na AWS.

---

## Gerenciamento de Custos (Cost Management)

* **AWS Cost and Usage Report:** Contém o conjunto mais abrangente de dados de custo e uso da AWS disponíveis, incluindo metadados adicionais sobre serviços, preços e reservas.
* **AWS Budgets:** Permite definir orçamentos personalizados que o alertam quando seus custos ou uso da AWS excedem (ou a previsão indica que excederão) o valor orçado.
* **AWS Cost Explorer:** Possui uma interface fácil de usar que permite visualizar, entender e gerenciar seus custos e uso da AWS ao longo do tempo.

---

## Gerenciamento e Governança (Management & Governance)

* **AWS Management Console:** Uma interface de usuário baseada na web para acessar sua conta AWS.
* **AWS Config:** Um serviço que ajuda a rastrear o inventário de recursos e as alterações.
* **Amazon CloudWatch:** Permite monitorar recursos e aplicações.
* **AWS Auto Scaling:** Fornece recursos que permitem escalar múltiplos recursos para atender à demanda.
* **AWS Command Line Interface (CLI):** Uma ferramenta unificada para gerenciar os serviços da AWS via linha de comando.
* **AWS Trusted Advisor:** Uma ferramenta online que ajuda a otimizar o desempenho e a segurança usando as melhores práticas da AWS.
* **AWS Well-Architected Tool:** Fornece ajuda na revisão e melhoria de suas cargas de trabalho (workloads).
* **AWS CloudTrail:** Um serviço que rastreia a atividade do usuário e o uso de APIs em suas contas da AWS.

# Revisão do Módulo e Análise de Questão Prática

## Revisão dos Tópicos Aprendidos

Neste módulo, você aprendeu a:
* Identificar a diferença entre **Regiões da AWS**, **Zonas de Disponibilidade** e **Locais de Borda (Edge Locations)**.
* Identificar os **serviços e as categorias de serviços** da AWS.

---

## Análise de Questão Prática (Exemplo de Exame)

### A Pergunta

> "Qual componente da infraestrutura global da AWS o Amazon CloudFront utiliza para garantir a entrega com baixa latência?"

### Decompondo a Pergunta

Para chegar à resposta correta, é preciso analisar as palavras-chave:

1.  **"Componente da infraestrutura global da AWS"**:
    * Isso indica que o foco da questão é em algo que a **AWS fornece**, e não em um recurso que um cliente possa criar ou configurar em sua própria conta.

2.  **"CloudFront"**:
    * É importante saber qual serviço da AWS a questão está abordando, neste caso, o serviço de entrega de conteúdo.

3.  **"Garantir a entrega com baixa latência"**:
    * Este é o benefício-chave. O uso de outro serviço poderia depender de um benefício diferente (ex: alta disponibilidade, recuperação de desastres). O termo "baixa latência" é a principal pista para o componente que estamos procurando.

### A Resposta Correta

Usando as informações da questão, podemos determinar que a resposta correta é:

**B) Locais de Borda da AWS (AWS Edge Locations)**
