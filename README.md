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

## Módulo 1: Visão Geral dos Conceitos de Nuvem

Bem-vindo(a) ao repositório de estudos para o curso **AWS Academy Cloud Foundations**!

Este espaço foi criado para centralizar e resumir o conteúdo do curso, servindo como uma fonte de consulta rápida para os principais conceitos de cada módulo.

Este primeiro módulo, **Visão Geral dos Conceitos de Nuvem**, estabelece a base para todo o curso, introduzindo conceitos fundamentais e as principais vantagens da computação em nuvem.

### Tópicos Abordados

* **Introdução à Computação em Nuvem:** O que é e por que a nuvem se tornou tão essencial.
* **As Seis Vantagens da Nuvem:** Uma visão geral dos principais benefícios de adotar a nuvem.
* **Visão Geral da AWS:** Conhecendo os principais serviços e categorias da Amazon Web Services.
* **AWS Cloud Adoption Framework (CAF):** Um guia estratégico para a adoção da nuvem.

---

### O que é Computação em Nuvem?

**Computação em Nuvem** é a entrega de serviços de TI sob demanda (como poder de computação, armazenamento e bancos de dados) pela internet, com pagamento por uso. Em vez de comprar e manter servidores físicos, você aluga recursos de um provedor como a AWS.

#### Modelo Tradicional vs. Nuvem

* **Modelo Tradicional:** Requer um alto investimento inicial (despesa de capital) em hardware. A capacidade é fixa e muitas vezes superdimensionada para picos de demanda, o que gera custos com recursos ociosos. É um processo demorado e inflexível.
* **Modelo de Nuvem:** Flexível, com pagamento apenas pelo que você usa. Permite aumentar ou diminuir a capacidade de forma automática, evitando gastos com recursos parados. Transforma a infraestrutura de hardware em algo flexível como um software.

---

### Tipos de Modelos

A nuvem tem três modelos principais de serviço e três de implantação, cada um com diferentes níveis de controle e flexibilidade:

#### **Modelos de Serviço (O que você gerencia?)**

* **IaaS (Infrastructure as a Service):** Oferece os blocos de construção básicos, como servidores virtuais e armazenamento. Você tem o maior controle sobre seus recursos, similar a uma infraestrutura tradicional.
* **PaaS (Platform as a Service):** Remove a necessidade de gerenciar o hardware e o sistema operacional. Você se concentra no desenvolvimento e implantação de suas aplicações.
* **SaaS (Software as a Service):** Entrega um produto completo e pronto para uso, gerenciado totalmente pelo provedor. É o caso de aplicativos de e-mail online, onde você só se preocupa em usar o serviço.

#### **Modelos de Implantação (Onde sua aplicação roda?)**

* **Nuvem (Cloud):** A aplicação é totalmente hospedada no ambiente do provedor de nuvem.
* **Híbrido (Hybrid):** Combina o ambiente local (on-premises) com a nuvem, conectando os dois.
* **Local (On-premises):** Conhecido como "nuvem privada", onde você usa as tecnologias de virtualização em sua própria infraestrutura física.

### Correspondência entre AWS e Infraestrutura Tradicional

O texto destaca que, embora a nuvem seja um novo paradigma, muitos de seus serviços têm equivalentes na infraestrutura tradicional de TI. Entender essa correspondência é fundamental para a transição.

* **Grupos de Segurança (Security Groups) e Listas de Controle de Acesso de Rede (Network ACLs):** Funcionam como **firewalls**, controlando o tráfego de entrada e saída de dados.
* **Identity and Access Management (IAM):** É similar ao **provisionamento de usuários** e **listas de controle de acesso** para gerenciar permissões.
* **Elastic Load Balancing (ELB) e Amazon Virtual Private Cloud (VPC):** Representam a **infraestrutura de rede** na nuvem, como **roteadores**, **switches** e **redes** em um ambiente físico.
* **Amazon Machine Images (AMIs):** São usadas para inicializar instâncias do Amazon EC2 e são o equivalente a **servidores virtuais on-premises**.
* **Amazon Elastic Block Store (EBS):** Atua como um disco rígido virtual para máquinas EC2, similar ao **armazenamento de conexão direta**.
* **Amazon Elastic File System (EFS):** Representa uma **Rede de Área de Armazenamento (SAN)** tradicional.
* **Amazon Simple Storage Service (S3):** Permite armazenar arquivos usando a internet, equivalente a um **armazenamento conectado à rede (NAS)**.
* **Amazon Relational Database Service (RDS):** É o equivalente a um **sistema de gerenciamento de banco de dados relacional (SGBDR)** físico.

Esses exemplos mostram que praticamente tudo que você faria em um data center tradicional é possível com a AWS. A diferença é que a AWS oferece tudo como um serviço, tirando de você a responsabilidade da infraestrutura física.

### As Seis Vantagens da Nuvem

A adoção da computação em nuvem oferece seis benefícios principais, que transformam a forma como a tecnologia é usada e gerenciada.

1.  **Troca de Despesa de Capital por Despesa Variável (CAPEX por OPEX):** Em vez de grandes investimentos iniciais em hardware (CAPEX), você paga apenas pelo que consome (OPEX). Na nuvem, você paga apenas pelo tempo e pela quantidade de recursos que utiliza, o que gera economia e flexibilidade.
2.  **Economia de Escala Massiva:** Ao usar a nuvem, você se beneficia da economia de escala de um provedor como a AWS, que atende a centenas de milhares de clientes. Essa escala permite que a AWS compre equipamentos a um custo muito mais baixo, o que resulta em preços menores para você.
3.  **Pare de Adivinhar a Capacidade:** Elimine a necessidade de prever a demanda máxima. Com a nuvem, você pode acessar a quantidade de recursos que precisar e escalar para cima ou para baixo em minutos, evitando recursos ociosos ou falta de capacidade.
4.  **Aumento da Velocidade e Agilidade:** Recursos de TI estão a um clique de distância. Isso reduz o tempo para disponibilizar recursos de semanas para minutos, permitindo que sua organização seja mais ágil e acelere o desenvolvimento e a experimentação.
5.  **Pare de Manter Data Centers:** Concentre-se no seu negócio, não na infraestrutura. A nuvem elimina o trabalho manual e repetitivo de gerenciar servidores (como "racking, stacking e powering"), liberando tempo e dinheiro para focar em projetos estratégicos.
6.  **Torne-se Global em Minutos:** Com a AWS, é possível implantar sua aplicação em múltiplas regiões geográficas no mundo com poucos cliques. Isso melhora a experiência do cliente ao reduzir a latência e o custo para sua empresa.

### Visão Geral da Amazon Web Services (AWS)

#### O que é um Serviço Web?

Um **serviço web** é uma aplicação disponibilizada e acessada pela internet. Ele usa formatos padronizados como **XML** ou **JSON** para receber e enviar dados, interagindo através de uma **Application Programming Interface (API)**. A grande vantagem é que ele não está vinculado a sistemas operacionais ou linguagens de programação, tornando-se uma peça de software autodescritiva e acessível pela rede.

A **AWS** é uma plataforma segura que oferece um ecossistema de **serviços web** sob demanda. Estes serviços, acessíveis pela internet, fornecem recursos de TI como computação, armazenamento, banco de dados e rede. Eles funcionam como blocos de construção que você pode interligar para criar soluções sofisticadas e escaláveis.

#### Benefícios Chave da AWS

A flexibilidade da AWS permite que você reconfigure, atualize e escale seu ambiente de forma automática, otimizando os gastos ao pagar apenas pelo que usa (modelo de despesa operacional, ou **OPEX**). O faturamento se torna uma despesa variável, não de capital.

#### Principais Categorias e Serviços

Os serviços da AWS são organizados em categorias, e a sua escolha depende dos objetivos de negócio e requisitos técnicos.

* **Serviços de Computação:**
    * **Amazon EC2:** Para quando você precisa de controle total sobre seus recursos.
    * **AWS Lambda:** Permite rodar código sem gerenciar servidores.
    * **AWS Elastic Beanstalk:** Gerencia e escala automaticamente suas aplicações web.
    * **Amazon Lightsail:** Uma plataforma simplificada para aplicações web básicas.
    * **AWS Batch:** Para executar centenas de milhares de cargas de trabalho em lote de forma confiável.
    * **AWS Outposts:** Para rodar a infraestrutura da AWS no seu próprio data center.
    * **Containers e Microsserviços:** **Amazon Elastic Container Service (ECS)**, **Amazon Elastic Kubernetes Service (EKS)** e **AWS Fargate**.
    * **VMware Cloud on AWS:** Para integrar seus serviços VMware existentes.

Outras categorias importantes incluem:
* Armazenamento
* Banco de Dados
* Rede
* Entrega de Conteúdo
* Segurança, Identidade e Conformidade
* Gerenciamento de Custos e Governança

#### Formas de Acessar a AWS

Você pode interagir com a vasta gama de serviços da AWS de três maneiras principais, todas construídas sobre uma API REST:

1.  **AWS Management Console:** Uma interface gráfica rica e intuitiva, acessível via navegador web.
2.  **AWS Command Line Interface (CLI):** Um conjunto de utilitários para automatizar a interação com o ecossistema por meio de scripts de comando.
3.  **Software Development Kits (SDKs):** Kits para desenvolvedores que permitem interagir com a AWS usando linguagens de programação como Java, C#, Python, Node.js, entre outras.

---

### O AWS Cloud Adoption Framework (AWS CAF)

O AWS CAF é um documento que ajuda organizações a planejar e executar uma migração bem-sucedida para a nuvem. A adoção da nuvem não é apenas sobre tecnologia; ela exige o alinhamento de **pessoas**, **processos** e **tecnologia** em toda a organização.

O framework ajuda a identificar lacunas em habilidades e processos e a construir uma abordagem abrangente para a adoção da nuvem em todo o ciclo de vida da TI.

#### As Seis Perspectivas do AWS CAF

O framework organiza a orientação em seis áreas de foco, conhecidas como **Perspectivas**. Cada uma delas é composta por capacidades que cobrem responsabilidades de equipes multifuncionais.

**Perspectivas de Negócio (Business Capabilities):**

1.  **Perspectiva de Negócios:** Inclui gerentes de negócios, gerentes de finanças e stakeholders de estratégia. O foco é criar um **caso de negócio** sólido para a adoção da nuvem e garantir que as estratégias de TI estejam alinhadas com as metas de negócio.
2.  **Perspectiva de Pessoas:** Inclui gerentes de RH, de pessoal e de pessoas. O framework ajuda a avaliar estruturas organizacionais e a identificar lacunas em habilidades e processos, priorizando treinamento, contratação e mudanças para construir uma organização ágil.
3.  **Perspectiva de Governança:** Inclui o CIO, gerentes de programa, arquitetos corporativos e analistas de negócios. Foca nas habilidades e processos necessários para alinhar as estratégias de TI e de negócio, maximizando o valor do investimento em TI e minimizando riscos.

**Perspectivas Técnicas (Technical Capabilities):**

4.  **Perspectiva de Plataforma:** Inclui o CTO, gerentes de TI e arquitetos de soluções. O foco é entender e comunicar a arquitetura de sistemas de TI. O framework oferece princípios e padrões para implementar novas soluções ou migrar cargas de trabalho para a nuvem.
5.  **Perspectiva de Segurança:** Inclui o CISO, gerentes e analistas de segurança de TI. O objetivo é garantir que a organização atenda aos objetivos de segurança, visibilidade, auditabilidade, controle e agilidade. O framework ajuda a estruturar a seleção e implementação de controles de segurança adequados.
6.  **Perspectiva de Operações:** Inclui gerentes de operações e suporte de TI. Define como as operações diárias, trimestrais e anuais são conduzidas. O framework ajuda a definir procedimentos operacionais atuais e a identificar as mudanças de processo e o treinamento necessários para uma adoção bem-sucedida da nuvem.

### Resumo do Módulo 1 e Questão de Exame

Este módulo abordou os conceitos fundamentais da computação em nuvem. Em resumo, você aprendeu a:

* Definir os diferentes tipos de modelos de computação em nuvem.
* Descrever as seis vantagens da nuvem.
* Reconhecer as principais categorias e serviços da AWS.
* Analisar o **AWS Cloud Adoption Framework (CAF)**.

---

### Análise de uma Questão de Certificação

O módulo finaliza com uma questão de exemplo para a certificação, que serve para testar a sua compreensão dos benefícios da nuvem.

**Pergunta:** Por que a AWS é mais econômica do que data centers tradicionais para aplicações com cargas de trabalho de computação variáveis?

**Análise da Pergunta:**
As palavras-chave são "**mais econômica**" e "**cargas de trabalho de computação variáveis**". A pergunta se refere a um dos seis benefícios da nuvem, especificamente aquele relacionado à flexibilidade e ao custo.

**Resposta Correta:**
A resposta é **C: A capacidade de iniciar instâncias sob demanda, quando necessário.**

**Justificativa:**
Em um data center tradicional, você precisa comprar recursos para lidar com o pico de demanda, mesmo que seja um evento raro. Isso resulta em custos elevados e recursos ociosos. Na AWS, a capacidade de **iniciar e encerrar instâncias dinamicamente** permite que você pague apenas pela capacidade que usa, tornando-se uma solução muito mais econômica para cargas de trabalho que variam.

### Módulo 2: Economia e Modelagem de Custos em Nuvem

Bem-vindo(a) ao Módulo 2! Este módulo foca nos aspectos financeiros e de custo da nuvem.

O objetivo principal é entender como a AWS precifica seus serviços e como você pode gerenciar e otimizar os gastos.

### Tópicos Abordados

* **Fundamentos de Preços da AWS:** Compreendendo a filosofia de precificação e suas características principais.
* **Custo Total de Propriedade (TCO):** Analisando os elementos do TCO e como usar a calculadora mensal da AWS.
* **Gerenciamento de Custos e Faturamento:** Como usar ferramentas como AWS Organizations para faturamento consolidado, além do Billing Dashboard, Cost Explorer, Budgets e relatórios de uso.
* **Planos de Suporte da AWS:** Uma visão geral das diferentes opções de suporte técnico disponíveis.

### Fundamentos de Preços da AWS

A filosofia de preços da AWS se baseia em três pilares principais, que permitem que a nuvem seja mais econômica e flexível que os data centers tradicionais.

1.  **Pague apenas pelo que usar:** Não há grandes despesas iniciais ou contratos de longo prazo. Você paga somente pelos serviços que consome e pelo tempo que os utiliza.
2.  **Pague menos quando usar mais:** O preço por unidade (por GB, por exemplo) diminui à medida que seu volume de uso aumenta, oferecendo descontos por volume.
3.  **Pague menos à medida que a AWS cresce:** A AWS investe em eficiência e repassa as economias de escala para os clientes, o que resulta em preços mais baixos ao longo do tempo.

#### Detalhes de Preços e Cobrança

O preço dos serviços da AWS é influenciado por três fatores: o **serviço** que você usa, o **volume de dados transferidos para fora da AWS** e a **região** onde o serviço está hospedado.

* A transferência de dados **para** a AWS é gratuita.
* A transferência de dados **entre serviços na mesma região** também é gratuita.
* A cobrança é feita no final do mês, baseada no uso. As transferências de dados de saída são agregadas e cobradas como "AWS data transfer out".

#### O AWS Free Tier (Nível Gratuito)

Para ajudar novos clientes, a AWS oferece o **AWS Free Tier**. Por até 12 meses, você pode usar serviços como o **Amazon EC2** (instâncias T2 micro), **Amazon S3** e **Amazon EBS** dentro de um limite de uso gratuito.

Além disso, alguns serviços como **Amazon VPC**, **AWS Elastic Beanstalk**, **Auto Scaling**, **AWS CloudFormation** e **AWS Identity and Access Management (IAM)** **não têm custo**. No entanto, lembre-se de que os recursos que esses serviços provisionam para você (como instâncias EC2) podem gerar cobranças.

### Custo Total de Propriedade (TCO)

O **TCO** é uma estimativa financeira que ajuda a comparar os custos diretos e indiretos de uma solução de TI. Ele é essencial para decidir entre uma implementação local (on-premises) e uma na nuvem.

#### Comparação: On-premises vs. Nuvem

* **Infraestrutura Local (On-premises):**
    * **Implantação:** Instalação em servidores próprios.
    * **Custos:** Baseados em **despesas de capital (CAPEX)**, que incluem custos fixos como instalações, hardware, licenças e equipe de manutenção.
    * **Flexibilidade:** A escalabilidade é cara e demorada. Diminuir a escala não reduz os custos fixos.
* **Infraestrutura em Nuvem (AWS):**
    * **Implantação:** Recursos adquiridos da AWS.
    * **Custos:** Baseados em **despesa variável**, que depende do uso do serviço.
    * **Flexibilidade:** A escalabilidade é simples e os custos são fáceis de estimar.

#### Calculadora de Custo Total de Propriedade (TCO Calculator)

É uma ferramenta da AWS para comparar uma implementação física com seu equivalente na nuvem. Ela ajuda a justificar financeiramente a migração, destacando que a nuvem geralmente tem custos iniciais mais baixos e custos operacionais reduzidos.

* **Exemplo Prático:** Uma solução on-premises de 3 anos pode custar mais de $100.000, enquanto uma equivalente na nuvem custa cerca de $7.000, representando uma economia de 96%.
* **Vantagem da Nuvem:** Na nuvem, você provisiona recursos apenas quando precisa e os desativa quando não são mais necessários, evitando o custo de capacidade ociosa.

#### Calculadora Simples de Custo Mensal (Simple Monthly Calculator)

Esta é outra ferramenta da AWS para dar transparência aos preços. Ela permite estimar o custo mensal de uma solução de nuvem proposta, e você pode adicionar, modificar ou remover serviços para ver como o custo muda.

* **Funcionalidade:**
    * Ajuda a estimar custos mensais de serviços.
    * Identifica oportunidades de redução de custo.
    * Usa modelos de implantação comuns.

Essas duas calculadoras são recursos valiosos para planejar e gerenciar seus custos na AWS.

### Estudo de Caso: Delaware North e a Economia de Custos na Nuvem

Este estudo de caso demonstra como o **Custo Total de Propriedade (TCO)** se aplica na prática, usando a migração da empresa Delaware North para a AWS.

#### O Problema

A Delaware North, uma líder global em serviços de alimentação, enfrentava um problema com seu data center local (on-premises): ele estava se tornando caro e ineficiente. A empresa precisava de um ambiente mais ágil para inovar e atender às demandas dos clientes.

#### O Processo de Avaliação

Em 2013, a empresa migrou 50 de seus sites para a AWS para uma fase de testes. A decisão de migrar totalmente para a nuvem foi baseada em três critérios principais:

1.  **Tecnologia:** A solução de nuvem precisava de um conjunto de tecnologias robusto para suportar todas as cargas de trabalho empresariais.
2.  **Operação:** A empresa buscava flexibilidade para otimizar processos internos e reduzir custos.
3.  **Finanças:** A migração precisava demonstrar um retorno sobre o investimento (ROI) claro.

#### Os Resultados da Migração para a AWS

A análise de TCO realizada pela Delaware North confirmou um resultado impressionante:

* **Economia Financeira:** A empresa projetou uma economia de **$3,5 milhões** em cinco anos.
* **Redução de Hardware:** Reduziu seu hardware físico em mais de **90%**, eliminando um total de **205 servidores**.
* **Agilidade e Velocidade:** O tempo para provisionar novas unidades de negócio foi reduzido de **2-3 semanas para apenas um dia**.
* **Outros Benefícios:** A empresa também observou melhorias em **consolidação de dados**, **conformidade de segurança** e **recuperação de desastres**.

Este caso de estudo prova que o modelo de "pague pelo que usar" da AWS não apenas reduz custos, mas também aumenta a agilidade e permite que as empresas se concentrem em inovar.

### AWS Organizations e Gerenciamento de Contas

O **AWS Organizations** é um serviço gratuito de gerenciamento que permite consolidar várias contas da AWS em uma única organização, facilitando o gerenciamento e o faturamento.

#### Por que usar o AWS Organizations?

* **Faturamento Consolidado:** Ele agrupa o faturamento de várias contas, tornando a visualização de custos por departamento ou equipe mais clara.
* **Gerenciamento de Segurança:** Permite aplicar controles de segurança a uma ou mais contas de forma centralizada.

#### Estrutura do AWS Organizations

A estrutura do Organizations é hierárquica, como uma árvore de cabeça para baixo com a **raiz (root)** no topo.

* **Raiz (Root):** A conta principal que gerencia toda a organização.
* **Unidade Organizacional (OU):** Uma ramificação que pode conter outras OUs e contas. Cada conta pode pertencer a apenas uma OU.
* **Contas:** Contas padrão da AWS que contêm seus recursos.

#### Comparação: IAM vs. Service Control Policies (SCPs)

É importante notar a diferença entre as políticas de **IAM** e as **SCPs**:

* **Políticas IAM:** Permitem ou negam o acesso a serviços da AWS, mas são aplicadas apenas a usuários, grupos ou funções IAM dentro de uma única conta.
* **Políticas de Controle de Serviço (SCPs):** Permitem ou negam o acesso a serviços específicos diretamente em uma conta ou em um grupo de contas (OU). Uma SCP restringe o acesso em um nível mais alto do que o IAM.

#### Como Configurar o AWS Organizations

Para configurar o serviço, siga estes passos:

1.  **Criar a Organização:** Use sua conta AWS atual como a conta principal e convide ou crie outras contas para se juntarem a ela.
2.  **Criar OUs:** Organize as contas em Unidades Organizacionais para agrupar e gerenciar melhor.
3.  **Criar SCPs:** Defina políticas de controle de serviço para restringir ações que podem ser delegadas a usuários e funções nas contas membro.
4.  **Testar as Políticas:** Use o IAM Policy Simulator ou faça login nas contas para garantir que as políticas funcionem conforme o esperado.

#### Formas de Gerenciar o AWS Organizations

Você pode gerenciar sua organização usando diversas interfaces, todas construídas sobre uma API REST:

1.  **AWS Management Console:** Interface gráfica via navegador.
2.  **AWS Command Line Interface (CLI):** Ferramenta de linha de comando para automação.
3.  **Software Development Kits (SDKs):** Bibliotecas e código de exemplo para desenvolvedores interagirem com a AWS via linguagens de programação.
4.  **HTTPS Query API:** Permite acesso programático direto ao servidor para requisições HTTPS.

### Ferramentas de Faturamento e Gerenciamento de Custos da AWS

O serviço **Billing and Cost Management** é o hub central para pagar sua fatura, monitorar o uso e orçar suas despesas na AWS. Ele oferece ferramentas para prever custos futuros e analisar tendências de uso com granularidade diária ou mensal.

#### Principais Ferramentas de Gerenciamento de Custos

1.  **AWS Billing Dashboard (Painel de Faturamento):**
    * Fornece uma visão geral do seu status de gastos no mês até a data.
    * Ajuda a identificar os serviços que mais contribuem para sua fatura.
    * Inclui gráficos como o **Resumo de Gastos (Spend Summary)**, que compara os gastos do mês anterior com as estimativas e previsões para o mês atual.
    * Apresenta o gráfico de **Gasto do Mês por Serviço**, mostrando os serviços mais caros em proporção ao seu custo total.

2.  **AWS Bills (Faturas da AWS):**
    * Exibe os custos incorridos no último mês para cada serviço.
    * Oferece um detalhamento por região da AWS e por contas vinculadas.
    * Permite acesso às informações mais atualizadas sobre seus custos e uso.

3.  **AWS Cost Explorer (Explorador de Custos):**
    * Uma ferramenta visual que ajuda a entender e gerenciar seus custos e uso da AWS ao longo do tempo.
    * Inclui relatórios padrão, como o de **Custos Mensais Correntes**, que visualiza os gastos dos últimos três meses e fornece previsões para o próximo.

4.  **AWS Budgets (Orçamentos):**
    * Permite criar orçamentos personalizados para monitorar seus gastos.
    * Envia notificações via e-mail ou **Amazon Simple Notification Service (Amazon SNS)** quando os gastos excedem os limites definidos.
    * Orçamentos podem ser rastreados em nível mensal, trimestral ou anual.

5.  **AWS Cost and Usage Report (Relatório de Custo e Uso):**
    * É a fonte de informação mais abrangente sobre seus custos e uso.
    * Lista o uso de cada serviço em itens de linha horários ou diários.
    * Pode ser configurado para publicar relatórios de faturamento em um bucket S3, com atualizações diárias.

Essas ferramentas trabalham juntas para dar a você total transparência e controle sobre seus gastos na nuvem.

### Como Usar as Ferramentas do Painel de Faturamento da AWS

O **AWS Billing Dashboard** é a sua central de controle para monitorar, analisar e gerenciar os custos da sua conta. Ele oferece uma visão completa e detalhada dos seus gastos.

#### 1. Acessando o Painel de Faturamento

* Na página inicial da AWS, clique no menu de conta e selecione **My Billing Dashboard**.
* O painel exibirá um resumo dos seus custos no mês, os serviços que mais gastam e uma previsão de gastos futuros.

#### 2. Visualizando e Analisando Custos com o Cost Explorer

O **Cost Explorer** permite mergulhar fundo nos seus dados de custo.
* **Acesso:** Clique em **Cost Explorer** no painel de faturamento.
* **Análise de Tendências:** Veja os custos atuais, previstos para o final do mês e compare com meses anteriores para identificar aumentos ou diminuições.
* **Explorando Detalhes:** Use as categorias para detalhar os custos por **região**, **tipo de instância** ou **serviço**. Por exemplo, é possível descobrir qual região está gerando mais custos ou qual tipo de instância específica é mais cara.
* **Criando e Salvando Relatórios:** Você pode criar relatórios personalizados (como "custos do acumulado do ano") e salvá-los para acesso rápido no futuro.

#### 3. Gerenciando Orçamentos com o AWS Budgets

O **AWS Budgets** ajuda a controlar os gastos e evitar surpresas.
* **Configuração:** Crie orçamentos para custos ou uso de serviço (por exemplo, um orçamento de $300 mensais).
* **Alertas:** Defina alertas para ser notificado (via e-mail ou SNS) quando seus custos ou uso excederem um certo limite (por exemplo, 90% do orçamento).
* **Lembre-se:** Os alertas apenas notificam você; eles não desligam os serviços automaticamente.

#### 4. Outras Ferramentas de Faturamento

* **AWS Bills:** Para uma fatura detalhada, com custos listados por serviço e por região.
* **AWS Cost and Usage Report:** Para relatórios mais granulares, com informações de uso por hora ou por dia, que podem ser enviados para um bucket S3.

Usar essas ferramentas permite que você tenha total visibilidade e controle sobre seus gastos na nuvem.

### Planos de Suporte Técnico da AWS

O suporte da AWS oferece uma combinação de ferramentas e expertise para ajudar a planejar, implantar e otimizar suas soluções com confiança.

#### Ferramentas e Funções de Suporte

* **Support Concierge:** Um especialista em faturamento e contas que oferece análise rápida e eficiente para questões não-técnicas.
* **AWS Trusted Advisor:** Um serviço automatizado que age como um especialista em nuvem, verificando seu ambiente para identificar oportunidades de redução de custos, melhoria de desempenho e segurança. É um recurso essencial para seguir as melhores práticas.
* **Technical Account Manager (TAM):** Um ponto de contato dedicado, disponível apenas no **Plano Enterprise**, que fornece orientação proativa, revisão de arquitetura e comunicação contínua.

#### Os Quatro Planos de Suporte

A AWS oferece quatro planos para atender a diferentes necessidades. Os planos que não são o Basic oferecem casos de suporte técnico ilimitados, sem contratos de longo prazo.

1.  **Plano Basic (Gratuito):**
    * Suporte para questões de faturamento e conta.
    * Suporte para aumentos de limite de serviço.
    * **Não inclui suporte para casos técnicos.**

2.  **Plano Developer:**
    * Acesso a orientações sobre melhores práticas.
    * Ferramentas de diagnóstico.
    * Suporte de arquitetura de blocos de construção.

3.  **Plano Business:**
    * Acesso completo ao **AWS Trusted Advisor**.
    * Orientação sobre casos de uso.
    * Acesso a uma API para gerenciamento automatizado de casos de suporte e operações do Trusted Advisor.

4.  **Plano Enterprise:**
    * Inclui todos os benefícios do Plano Business.
    * **Acesso exclusivo a um Technical Account Manager (TAM).**
    * Roteamento de caso "white glove" (tratamento especial).
    * Orientação de arquitetura de aplicação.
    * Revisões de negócios gerenciais.
    * Suporte de gerenciamento de eventos de infraestrutura.

#### Níveis de Gravidade de Casos

A **Gravidade** define o tipo de resposta que você receberá, independentemente do seu plano (exceto o Basic, que não tem suporte técnico para casos).

1.  **Crítico:** O negócio está em risco; funções críticas da aplicação estão indisponíveis.
2.  **Urgente:** O negócio é significativamente impactado; funções importantes da aplicação estão indisponíveis.
3.  **Alto:** Funções importantes da aplicação estão prejudicadas ou degradadas.
4.  **Normal:** Funções não-críticas se comportam de forma anormal ou há uma pergunta de desenvolvimento sensível ao tempo.
5.  **Baixo:** Uma pergunta de desenvolvimento geral ou solicitação de recurso.

A escolha do plano de suporte deve considerar tanto os custos e recursos quanto os tempos de resposta esperados para cada nível de gravidade.

### Resumo do Módulo 2 e Questão de Exame

Este módulo aprofundou na **economia e nos custos da nuvem**. Em resumo, você aprendeu sobre:

* Os **fundamentos de preços** da AWS.
* O conceito de **Custo Total de Propriedade (TCO)**.
* As ferramentas **AWS Simple Monthly Calculator** e **AWS TCO Calculator**.
* As ferramentas de **Faturamento e Gerenciamento de Custos** (Billing Dashboard, Cost Explorer, Budgets).
* Os **quatro planos de suporte** da AWS (Basic, Developer, Business, Enterprise).

O objetivo principal é que você possa planejar, implantar e otimizar suas soluções com confiança, escolhendo o plano e as ferramentas que melhor atendem às suas necessidades.

---

### Análise de uma Questão de Certificação

A seguir, um exemplo de questão de exame para praticar o que foi aprendido:

**Pergunta:** Qual serviço da AWS oferece recomendações de otimização de segurança da infraestrutura?

**Análise:**
A palavra-chave na pergunta é "**recomendações**". Isso aponta para um serviço que não apenas mostra o status, mas também dá conselhos para melhorar sua infraestrutura.

**Resposta Correta:**
A resposta é **C: Trusted Advisor**.

**Justificativa:**
O **AWS Trusted Advisor** é o serviço que fornece orientações em tempo real para ajudar você a provisionar recursos seguindo as melhores práticas da AWS. Ele é um recurso online que ajuda a reduzir custos, aumentar o desempenho e **melhorar a segurança** ao otimizar seu ambiente AWS.

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
* Regiões;
* Zonas de disponibilidade;
* Pontos de presença (que incluem os locais de borda).

Essa infraestrutura fornece a plataforma para um vasto conjunto de serviços, como redes, armazenamento, serviços de computação e bancos de dados.

Esses serviços são entregues como um utilitário sob demanda (on-demand), disponível em segundos, com preços no modelo pague-pelo-uso (pay-as-you-go).

### Foco do Curso

Existem 23 categorias diferentes de produtos ou serviços, e cada categoria consiste em um ou mais serviços. Este curso não tentará apresentar cada um deles. Em vez disso, o foco é nos serviços mais amplamente utilizados e que oferecem a melhor introdução à Nuvem AWS. O curso também se concentra nos serviços que têm maior probabilidade de serem abordados no exame AWS Certified Cloud Practitioner.

---

## Serviços de Armazenamento (Storage)

* **Amazon Simple Storage Service (Amazon S3):** Um serviço de armazenamento de objetos que oferece escalabilidade, disponibilidade de dados, segurança e desempenho.
* **Amazon Elastic Block Store (Amazon EBS):** Um armazenamento em bloco de alto desempenho projetado para uso com o Amazon EC2, tanto para cargas de trabalho intensivas em taxa de transferência (throughput) quanto em transações.
* **Amazon Elastic File System (Amazon EFS):** Fornece um sistema de arquivos de rede (Network File System - NFS) elástico, escalável e totalmente gerenciado para uso com serviços na Nuvem AWS e recursos on-premises.
* **Amazon S3 Glacier:** Uma classe de armazenamento do Amazon S3 segura, durável e de custo extremamente baixo, ideal para arquivamento de dados e backup de longo prazo.

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
