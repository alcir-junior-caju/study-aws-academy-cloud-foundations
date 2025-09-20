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

# Módulo 4: Segurança na Nuvem AWS

### A Importância Crítica da Segurança
A segurança é a maior prioridade na AWS. Uma vulnerabilidade pode destruir anos de trabalho e causar perdas financeiras significativas, devendo ser a conversa inicial e principal em qualquer projeto de TI. A AWS fornece as ferramentas, o suporte e a documentação para ajudar a proteger seus dados, sistemas e aplicações.

---

### Tópicos Abordados no Módulo
* O Modelo de Responsabilidade Compartilhada da AWS.
* AWS Identity and Access Management (IAM).
* Como proteger uma nova conta AWS.
* As melhores formas de proteger seus dados.
* Recursos disponíveis para garantir a conformidade (compliance).

---

### Recursos de Aprendizagem Disponíveis
* **Demonstração Gravada:** Focada em Identity and Access Management (IAM).
* **Laboratório Prático (Hands-on):** Para praticar a configuração de usuários e políticas do IAM.
* **Verificação de Conhecimento:** Para testar a compreensão dos conceitos-chave.

---

### Objetivos de Aprendizagem
Ao final deste módulo, você será capaz de:
* **Reconhecer o Modelo de Responsabilidade Compartilhada:** Identificar o que é responsabilidade da AWS e o que é responsabilidade do cliente.
* **Entender o IAM:** Saber o que são usuários, grupos, funções (roles) e políticas.
* **Proteger Contas:** Compreender as melhores práticas para proteger suas contas AWS.
* **Proteger Dados:** Saber como proteger os dados "em trânsito" (movendo-se entre sistemas) e "em repouso" (armazenados).

# O Modelo de Responsabilidade Compartilhada da AWS

## O Princípio Fundamental: "DA" Nuvem vs. "NA" Nuvem

Segurança e conformidade são uma responsabilidade compartilhada entre a AWS e os clientes. O modelo basicamente indica quais partes da segurança serão tratadas pela AWS e de quais partes os clientes são responsáveis. A distinção principal é:

* **AWS é responsável pela segurança DA nuvem.**
* **O Cliente é responsável pela segurança NA nuvem.**

A AWS fornece as ferramentas para proteger suas aplicações e dados. No entanto, é sua responsabilidade usar essas ferramentas corretamente.

---

## Responsabilidade da AWS: Segurança DA Nuvem

A AWS opera, gerencia e controla desde a camada de virtualização de software até a segurança física das instalações onde os serviços operam. As responsabilidades da AWS incluem:

* **Infraestrutura Global:** Proteger a infraestrutura que executa todos os serviços da nuvem AWS, o que inclui o hardware, software, redes e as instalações. Isso abrange:
    * Regiões da AWS
    * Zonas de Disponibilidade
    * Locais de Borda (Edge Locations)
* **Segurança Física:** Proteger a segurança física dos data centers e da infraestrutura que hospeda os seus recursos.
* **Manutenção e Redundância:** Garantir a redundância da infraestrutura e operar a detecção de intrusão.
* **Isolamento de Virtualização:** Assegurar que a infraestrutura de virtualização forneça isolamento entre as cargas de trabalho dos diferentes clientes. Por exemplo, as instâncias EC2 de um cliente são isoladas da computação de outro cliente.

---

## Responsabilidade do Cliente: Segurança NA Nuvem

Como cliente, você é responsável pelo que você implanta ao usar os serviços da AWS. As etapas de segurança específicas dependem dos serviços utilizados e da complexidade das suas aplicações. Suas responsabilidades incluem:

* **Dados do Cliente:** Você mantém controle completo sobre seus dados, o que inclui:
    * Decidir quais dados armazenar na nuvem AWS.
    * Definir quais serviços terão acesso aos dados.
    * Escolher as localizações geográficas onde os dados serão armazenados.
* **Criptografia:** Implementar a criptografia para proteger os dados:
    * **Em trânsito:** Enquanto se movem de um sistema para outro.
    * **Em repouso:** Quando estão armazenados.
* **Gerenciamento de Acesso e Credenciais:** Assegurar que as credenciais de segurança e os logins sejam gerenciados de forma segura.
* **Configuração de Rede:** Garantir que a rede esteja configurada para a máxima segurança, o que inclui:
    * Gerenciamento das configurações de firewall.
    * Configuração de Security Groups e outras definições de rede.
* **Sistema Operacional, Aplicações e Patches:** Em serviços como o Amazon EC2, você é responsável por:
    * Proteger e gerenciar o sistema operacional (instalar atualizações, patches de segurança, etc.).
    * Proteger as aplicações que você instala e executa.

---

## Como o Tipo de Serviço Altera a Responsabilidade

A quantidade de responsabilidade que você assume depende do tipo de serviço de nuvem que você utiliza.

### 1. Infraestrutura como Serviço (IaaS)
Refere-se a serviços onde você mantém o controle e o gerenciamento da maior parte do sistema.
* **Nível de Responsabilidade do Cliente:** Alto.
* **Exemplo:** Amazon EC2.
* **Detalhes:** Você recebe um servidor virtualizado e tem controle completo sobre ele, de forma muito semelhante a um servidor físico. Você gerencia o sistema operacional, decide qual software instalar e é responsável por toda a segurança a partir desse nível.

### 2. Plataforma como Serviço (PaaS)
Refere-se a serviços que utilizam a infraestrutura, mas ela é gerenciada pelo provedor de nuvem e fica, em grande parte, oculta para você.
* **Nível de Responsabilidade do Cliente:** Médio.
* **Exemplo:** Amazon Relational Database Service (RDS).
* **Detalhes:** A AWS opera e atualiza os servidores, o sistema operacional e automatiza os backups. Você não precisa se preocupar com aquisição de recursos, planejamento de capacidade, manutenção de software ou patches. Sua responsabilidade é focar no seu código e nos dados, acessando o serviço através de endpoints para armazenar e recuperar informações.

### 3. Software como Serviço (SaaS)
Refere-se a serviços que fornecem uma solução de software completa e pronta para uso. O software é hospedado e gerenciado centralmente pelo provedor.
* **Nível de Responsabilidade do Cliente:** Baixo.
* **Exemplos:** AWS Trusted Advisor, AWS Shield.
* **Detalhes:** Você, como cliente, não precisa gerenciar nenhuma parte da infraestrutura que suporta o serviço. O modelo de licenciamento é tipicamente por assinatura ou pague-pelo-uso.

## AWS Identity and Access Management (IAM)

### 1. O que é o IAM?

O Identity and Access Management é um dos primeiros serviços que você usará na AWS. É a ferramenta que gerencia centralmente o acesso para lançar, configurar, gerenciar e terminar recursos em sua conta AWS.

#### Características Principais:
* **Serviço Gratuito:** Não há cobrança para definir usuários, grupos, funções e controles de acesso.
* **Serviço Global:** Os recursos do IAM (como usuários e grupos) não são atrelados a uma região específica; eles estão disponíveis globalmente.
* **Controle Centralizado:** Permite controlar o acesso a todos os seus serviços AWS usando políticas.
* **Controle Granular:** Fornece um controle refinado sobre o acesso aos recursos, incluindo quem pode acessá-los e como podem ser acessados.

---

### 2. Os 4 Componentes Fundamentais do IAM

O IAM permite que você defina alguns itens essenciais:

* **Usuário (User):** Geralmente uma pessoa (ou aplicação) que foi autorizada a acessar sua conta AWS. Cada usuário deve ter um nome único (sem espaços) e uma forma de se identificar, como uma senha.

* **Grupo (Group):** Um mecanismo para aplicar permissões a um conjunto de usuários. Você define um grupo, aplica uma política de acesso a ele e, em seguida, pode adicionar ou remover usuários desse grupo. Isso é útil para gerenciar permissões para equipes com diferentes responsabilidades (DBAs, desenvolvedores, auditores).

* **Política (Policy):** Um documento (em formato JSON) que define as permissões de acesso a um ou mais serviços. As políticas são anexadas a usuários, grupos ou funções para habilitar os controles de acesso que elas definem.

* **Função (Role):** Um mecanismo para conceder **acesso temporário** aos serviços da AWS. Um usuário ou serviço pode "assumir uma função" para obter permissões que normalmente não possui, executar uma tarefa e depois reverter ao seu acesso usual. É semelhante ao comando `sudo` no Linux.

---

### 3. Conceitos-Chave: Autenticação e Autorização

#### Autenticação: "Quem é você?"
É o processo em que um usuário ou sistema deve provar sua identidade antes de obter acesso. Ao definir um usuário no IAM, você pode atribuir dois tipos de acesso:

1.  **Acesso Programático:** Para acesso via API, AWS CLI ou SDKs. A autenticação é feita com um par de chaves:
    * ID da Chave de Acesso (Access Key ID)
    * Chave de Acesso Secreta (Secret Access Key)

2.  **Acesso ao Console de Gerenciamento da AWS:** Para acesso via interface web. A autenticação é feita com:
    * Nome de usuário
    * Senha

#### A Camada Extra de Segurança: Autenticação Multifator (MFA)
Para maior segurança, é altamente recomendado habilitar o MFA. Ele adiciona uma segunda camada de verificação, exigindo uma informação adicional (um código gerado em tempo real) além da senha. Mesmo que as credenciais sejam comprometidas, o acesso não será concedido sem o código MFA.
* **Opções de MFA:** Aplicações virtuais (Google Authenticator), chaves de segurança U2F (YubiKey) ou dispositivos de hardware MFA.

### Autorização: "O que você pode fazer?"
É o processo de determinar quais permissões um usuário ou serviço (já autenticado) deve ter.

* **Padrão de Acesso Zero:** Por padrão, usuários, grupos e funções do IAM são criados **sem permissão para nada**. Você deve conceder permissões explicitamente.

#### O Princípio do Menor Privilégio
Este é um conceito fundamental de segurança que promove a concessão do **conjunto mínimo de permissões** que um usuário precisa para realizar suas tarefas, e nada mais. Ao criar políticas no IAM, esta é a prática recomendada.

---

## 4. Políticas do IAM em Profundidade

Uma política do IAM é um documento JSON que lista permissões `Allow` (Permitir) ou `Deny` (Negar) para serviços na AWS.

### Tipos de Políticas
1.  **Políticas Baseadas em Identidade:** Anexadas a uma identidade (usuário, grupo ou função). Elas definem o que *aquela identidade pode fazer*.
2.  **Políticas Baseadas em Recursos:** Anexadas a um recurso (como um bucket S3). Elas definem quem pode acessar *aquele recurso específico*.

### A Lógica de Avaliação de Políticas (Regra de Ouro)
Quando uma ação é solicitada, o IAM avalia todas as políticas aplicáveis com a seguinte lógica:

1.  **Negação Implícita (Padrão):** Por padrão, todo acesso é negado.
2.  **Busca por uma Negação Explícita (`Deny`):** O IAM primeiro verifica se existe alguma política com uma declaração `Deny` para a ação. Se encontrar, o acesso é **imediatamente negado**.
3.  **Busca por uma Permissão Explícita (`Allow`):** Se não houver um `Deny` explícito, o IAM procura por uma política com uma declaração `Allow` para a ação. Se encontrar, o acesso é permitido.
4.  **Resultado Final:** Se não houver nem `Deny` nem `Allow` explícitos, a negação implícita padrão prevalece e o acesso é negado.

> **A regra mais importante:** Uma **negação explícita (`Deny`) sempre se sobrepõe a qualquer permissão explícita (`Allow`)**.

---

### 5. Grupos e Funções (Roles) em Detalhe

#### Grupos do IAM
* Um grupo é uma coleção de usuários. É uma forma de gerenciar permissões para múltiplos usuários de uma só vez.
* Um usuário pode pertencer a vários grupos.
* **Regra Importante:** Grupos **não podem ser aninhados** (um grupo não pode conter outro grupo). Eles contêm apenas usuários.
* Não existe um "grupo padrão" na AWS; você precisa criar e gerenciar todos os grupos.

#### Funções (Roles) do IAM
* Uma função é uma identidade com permissões específicas, mas **não está associada a uma única pessoa**. Ela é destinada a ser "assumível" por qualquer entidade (usuário, aplicação, serviço AWS) que precise dela.
* A principal diferença para um usuário é que uma função **não possui credenciais de longo prazo** (senha ou chaves de acesso permanentes).
* Ao assumir uma função, a entidade recebe **credenciais de segurança temporárias** para executar as tarefas permitidas por aquela função.

---

### 6. Exemplo Prático: Usando uma Role com EC2 e S3

Este cenário ilustra o poder das funções:

1.  **O Problema:** Uma aplicação rodando em uma instância EC2 precisa ler dados de um bucket S3 chamado "Photos".
2.  **A Solução (com Role):**
    * Um administrador cria uma **Função do IAM**.
    * A função recebe uma **política de permissão** que concede acesso de apenas leitura ao bucket "Photos".
    * A função também recebe uma **política de confiança** que especifica que a instância EC2 tem permissão para *assumir* esta função.
    * O administrador **anexa a função à instância EC2**.
3.  **O Resultado:**
    * Quando a aplicação na instância EC2 precisa acessar o S3, ela assume a função anexada.
    * Ela recebe **credenciais temporárias** com as permissões de leitura do bucket.
    * A aplicação usa essas credenciais para ler os dados do S3.

**Vantagem:** O desenvolvedor não precisou colocar chaves de acesso (credenciais de longo prazo) no código da aplicação, e o administrador não precisou dar permissões diretas ao desenvolvedor. É uma forma muito mais segura e gerenciável.

# Guia Prático do IAM: Como Fazer no Console da AWS

Este guia transforma a demonstração em vídeo em um passo a passo para você seguir.

---

## Tutorial 1: Como Criar uma Função (Role) para uma Instância EC2

**Objetivo:** Permitir que uma aplicação rodando em uma instância EC2 acesse outros serviços da AWS (como S3 e DynamoDB) de forma segura, sem precisar armazenar credenciais de acesso no código.

### Passo 1: Iniciar a Criação da Role
1.  No Console da AWS, navegue até o serviço **IAM**.
2.  No menu à esquerda, clique em **Funções (Roles)**.
3.  Clique no botão **Criar função (Create a Role)**.

### Passo 2: Selecionar a Entidade Confiável
1.  A "entidade confiável" é quem poderá assumir esta função. Para este caso, selecione **AWS Service**.
2.  No caso de uso, escolha **EC2**.
3.  Clique em **Próximo**.

### Passo 3: Adicionar Permissões (Anexar Políticas)
1.  Agora, você precisa definir o que a instância EC2 poderá fazer. Para isso, anexe políticas de permissão.
2.  Na barra de busca de políticas, digite `S3`.
3.  Selecione a política `AmazonS3ReadOnlyAccess` (para dar acesso de apenas leitura a todos os buckets S3).
4.  Na mesma barra de busca, agora digite `DynamoDB`.
5.  Selecione a política `DynamoDBReadOnlyAccess`.
6.  Clique em **Próximo**.

### Passo 4: Nomear e Criar a Role
1.  Dê um **Nome para a função** que seja descritivo. Ex: `MyAppRole`.
2.  Revise as políticas que você anexou (`AmazonS3ReadOnlyAccess` e `DynamoDBReadOnlyAccess`).
3.  Clique em **Criar função**.

### Passo 5: Atribuir a Role a uma Instância EC2
1.  Ao criar uma nova instância EC2 (no serviço EC2 > Lançar instância), avance até a etapa de **Configurar Detalhes da Instância**.
2.  Localize o campo **Função do IAM (IAM Role)**.
3.  No menu suspenso, selecione a role que você acabou de criar (`MyAppRole`).
4.  Prossiga com a criação da instância.

> **Resultado:** A instância EC2 lançada com esta role anexada herdará automaticamente as permissões para ler dados do S3 e do DynamoDB.

---

## Tutorial 2: Como Gerenciar Permissões com Grupos e Usuários

**Objetivo:** Gerenciar permissões de forma eficiente para uma equipe de usuários com as mesmas responsabilidades (ex: operadores de rede).

### Parte A: Criar o Grupo de Usuários

1.  No console do **IAM**, clique em **Grupos (Groups)** no menu à esquerda.
2.  Clique em **Criar novo grupo**.
3.  Dê um nome para o grupo. Ex: `NetOps`.
4.  Anexe a política de permissão necessária para a função do grupo. Para operadores de rede, por exemplo, pesquise e selecione `AmazonVPCFullAccess`.
5.  Clique em **Criar grupo**.

### Parte B: Criar um Usuário e Adicioná-lo ao Grupo

1.  No console do **IAM**, clique em **Usuários (Users)** no menu à esquerda.
2.  Clique em **Adicionar usuário**.
3.  Defina um **Nome de usuário**. Ex: `Dave`.
4.  Selecione o **Tipo de acesso**. Para este exemplo, marque **Acesso ao Console de Gerenciamento da AWS**.
5.  Configure as opções de senha (ex: senha gerada automaticamente com exigência de alteração no primeiro login).
6.  Na tela de **Permissões**, escolha a opção **Adicionar usuário ao grupo**.
7.  Selecione o grupo que você criou na Parte A (`NetOps`).
8.  Avance pelas etapas de revisão e clique em **Criar usuário**.

> **Resultado:** O usuário `Dave` agora possui acesso total à VPC. Ele herdou essa permissão diretamente do grupo `NetOps`, sem a necessidade de anexar a política diretamente a ele.

---

### Dica Pro: Políticas Personalizadas e o Menor Privilégio

Lembre-se, o IAM é baseado no **princípio do menor privilégio**: nenhuma entidade deve ter mais permissões do que o estritamente necessário para realizar seu trabalho.

* Nos exemplos acima, usamos políticas gerenciadas pela AWS (como `AmazonS3ReadOnlyAccess`).
* Para ser ainda mais seguro, você pode criar suas próprias políticas personalizadas usando o **Editor Visual** ou escrevendo o documento **JSON** diretamente. Isso permite restringir o acesso a recursos específicos (ex: apenas um bucket S3, em vez de todos).

# Checklist Essencial: Como Proteger uma Nova Conta AWS

## Parte 1: O Problema - O Perigo da Conta Raiz (Root)

Quando você cria uma conta AWS pela primeira vez, você começa com uma única identidade que tem acesso completo a todos os serviços da AWS. Essa identidade é chamada de **conta raiz da AWS (root account)**.

* **Acesso:** O login é feito com o endereço de e-mail e a senha que você usou para criar a conta.
* **Poderes:** A conta raiz tem acesso total e irrestrito a todos os recursos da conta.

> **AVISO IMPORTANTE:**
> A AWS recomenda fortemente que você **NÃO use esta conta para interações do dia a dia**.

A abordagem correta é usar o Identity and Access Management (IAM) para criar usuários, atribuir as permissões necessárias a eles e seguir o **princípio do menor privilégio**.

---

## Parte 2: Passos Imediatos para Proteger sua Conta

Siga esta sequência para parar de usar a conta raiz e estabelecer uma base de segurança sólida.

### Passo 1: Habilite o MFA na Conta Raiz
Este é um passo de segurança fundamental que deve ser feito o mais rápido possível. Habilitar a Autenticação Multifator (MFA) para a conta raiz protegerá a conta que está conectada ao seu cartão de crédito e detalhes financeiros.

### Passo 2: Crie seu Primeiro Usuário Administrativo no IAM
Para parar de usar a conta raiz, o primeiro passo é criar um usuário do IAM para si mesmo através do Console de Gerenciamento da AWS.

### Passo 3: Configure uma Política de Senhas (Password Policy)
Habilite uma política de senhas para todos os usuários. Isso reforça a segurança exigindo senhas mais fortes (comprimento mínimo, caracteres especiais, etc.).

### Passo 4: Crie um Grupo de Administradores
1.  No console do IAM, crie um novo grupo.
2.  Dê a ele um nome descritivo, como `acesso-administrativo`.
3.  Anexe a política gerenciada pela AWS chamada `AdministratorAccess`.

### Passo 5: Adicione seu Usuário ao Grupo de Administradores
Adicione o usuário IAM que você criou no Passo 2 a este novo grupo. Ele herdará todas as permissões de administrador.

### Passo 6: Remova as Chaves de Acesso (Access Keys) da Conta Raiz
Antes de começar a usar seu novo usuário, certifique-se de desabilitar e remover as chaves de acesso da sua conta raiz, se elas existirem. Elas concedem acesso programático e raramente são necessárias para o usuário root.

### Passo 7: Faça Logout da Raiz e Login com seu Usuário IAM
1.  No painel do console do IAM, copie o **link de login** específico da sua conta (ele tem um formato como `https://<ID_DA_CONTA>.signin.aws.amazon.com/console`).
2.  Faça **logout** como usuário root.
3.  Acesse o link de login que você copiou e entre no console usando suas novas credenciais de usuário IAM.

### Passo 8: Guarde as Credenciais da Conta Raiz em um Local Seguro
Não se esqueça de guardar as credenciais do seu usuário raiz e o dispositivo MFA em um local extremamente seguro e de acesso restrito.

---

## Parte 3: Próximos Passos Recomendados para Segurança Contínua

### Habilitar o MFA para seu Usuário Administrativo
Assim como fez para a conta raiz, ao fazer login com seu novo usuário administrador, habilite também a autenticação multifator para essa conta. O MFA também pode ser usado para proteger o acesso programático.

### Habilitar e Utilizar o AWS CloudTrail
O CloudTrail é um serviço que registra todas as solicitações de API feitas aos recursos em sua conta, habilitando a auditoria operacional.
* **Propósito:** É a base para responder "quem", "o quê", "quando" e "onde" sobre as interações de API, sendo fundamental para investigações de segurança e documentação de conformidade.
* **Padrão:** O CloudTrail já vem habilitado por padrão na criação da conta e armazena os últimos 90 dias de eventos de gerenciamento. Você pode configurar uma "trilha" para estender esse período de retenção.

### Habilitar Relatórios de Faturamento (Billing Reports)
É uma prática recomendada habilitar relatórios como o **Relatório de Custos e Uso da AWS (AWS Cost and Usage Report)**.
* **Propósito:** Fornecem informações detalhadas sobre o uso de recursos da AWS e os custos estimados, rastreando o uso e as cobranças por hora ou por dia.
* **Funcionamento:** Os relatórios são entregues pelo menos uma vez por dia em um bucket do Amazon S3 que você especificar.

# Guia de Segurança de Dados na AWS

## Parte 1: Criptografia de Dados

### O que é Criptografia?
A criptografia de dados é uma ferramenta essencial a ser usada quando você deseja proteger seus dados. Ela pega dados que são legíveis e os codifica para que se tornem ilegíveis para qualquer pessoa que não tenha acesso à chave secreta que foi usada para codificá-los. Mesmo que um invasor obtenha acesso aos seus dados, ele não conseguirá entendê-los.

### 1. Criptografia de Dados em Repouso (Data at Rest)
Refere-se a dados que estão fisicamente armazenados em disco, ou seja, não estão se movendo.
* Você pode criar sistemas de arquivos criptografados na AWS para que todos os seus dados e metadados sejam criptografados em repouso.
* O algoritmo padrão utilizado é o **Advanced Encryption Standard (AES-256)**.

#### Ferramenta Chave: AWS Key Management Service (KMS)
Quando você usa o AWS KMS, a criptografia e a descriptografia são tratadas de forma automática e transparente, para que você não precise modificar suas aplicações.
> **Recomendação:** Se sua organização estiver sujeita a políticas corporativas ou regulatórias que exigem a criptografia, a AWS recomenda habilitar a criptografia em todos os serviços que armazenam seus dados.

### 2. Criptografia de Dados em Trânsito (Data in Transit)
Refere-se a dados que estão se movendo através da rede.
* A criptografia é realizada usando o **Transport Layer Security (TLS 1.2)**, um padrão aberto que utiliza a cifra AES-256 (antigamente chamado de SSL).
* O tráfego da web sobre HTTP **não é seguro**. O tráfego sobre **HTTPS** é criptografado usando TLS/SSL, protegendo contra espionagem (eavesdropping) e ataques man-in-the-middle.

#### Ferramenta Chave: AWS Certificate Manager (ACM)
O ACM é um serviço que permite provisionar, gerenciar e implantar certificados SSL/TLS para uso com seus serviços AWS, como um **Load Balancer** ou **Distribuições CloudFront**. O serviço também lida com as renovações dos certificados.

#### Exemplos Práticos de Criptografia em Trânsito:
* **EC2 e EFS:** Todo o tráfego de dados entre uma instância EC2 e um sistema de arquivos Amazon EFS montado é criptografado usando TLS/SSL.
* **Storage Gateway e S3:** Quando o AWS Storage Gateway (um serviço de nuvem híbrido) se conecta ao Amazon S3 pela internet, a conexão criptografa os dados em trânsito.

---

## Parte 2: Controle de Acesso a Dados no Amazon S3

É essencial gerenciar e controlar o acesso aos dados do Amazon S3. Por padrão, **todos os buckets do Amazon S3 são privados** e só podem ser acessados por usuários que receberam acesso explicitamente. A AWS fornece várias ferramentas para isso.

### Métodos para Controlar o Acesso ao S3

#### 1. Bloqueio de Acesso Público do S3 (S3 Block Public Access)
* Este recurso se sobrepõe a qualquer outra política ou permissão de objeto.
* É **habilitado por padrão** quando você cria um novo bucket.
* Fornece um método direto e eficaz para evitar a exposição pública não intencional de dados.

#### 2. Políticas do IAM (Baseadas em Identidade)
* Você pode escrever políticas do IAM que especificam quais usuários ou funções (roles) podem acessar buckets e objetos específicos.

#### 3. Políticas de Bucket (Baseadas em Recurso)
* São políticas anexadas diretamente a um recurso (o bucket S3).
* São tipicamente usadas quando o usuário ou sistema não pode se autenticar via IAM, como para conceder **acesso entre contas da AWS** ou **acesso público/anônimo**.
* **Atenção:** Devem ser escritas com cuidado e totalmente testadas. Uma declaração de negação (`Deny`) em uma política de bucket restringirá o acesso, mesmo que o usuário tenha uma permissão `Allow` em sua política do IAM.

#### 4. Listas de Controle de Acesso (ACLs)
* É outra maneira de proteger os buckets, mas é um método mais antigo, anterior ao IAM.
* Seu uso é menos comum hoje em dia.
* **Atenção:** Se for usar ACLs, não defina um acesso que seja muito aberto ou permissivo.

---

## Parte 3: Ferramentas de Verificação de Segurança

### AWS Trusted Advisor
* Este serviço fornece uma funcionalidade de **verificação de permissão de bucket**.
* É uma ferramenta útil para descobrir se algum dos buckets em sua conta tem permissões que concedem acesso global.

# Guia de Conformidade (Compliance) na AWS

## O Compromisso da AWS com a Conformidade

A AWS se envolve com órgãos certificadores externos e auditores independentes para fornecer aos clientes informações sobre as políticas, processos e controles estabelecidos e operados pela empresa.

A conformidade especifica os requisitos para estabelecer, implementar, manter e melhorar continuamente um **Sistema de Gerenciamento de Segurança da Informação**. Os requisitos de certificação envolvem o desenvolvimento e a implementação de um programa de segurança rigoroso. Este sistema define como a AWS gerencia a segurança de maneira holística e abrangente.

Além disso, a AWS fornece recursos de segurança e acordos legais projetados para ajudar a dar suporte aos clientes com regulamentações e leis comuns. Um exemplo é a **Lei de Portabilidade e Responsabilidade de Seguros de Saúde (HIPAA)**.

---

## Ferramenta 1: AWS Config - Para Auditoria de Configuração

### O que é?
O AWS Config é um serviço que você pode usar para **avaliar, auditar e analisar a configuração** dos seus recursos da AWS. Ele mantém um histórico da sua configuração e permite que você defina quem pode mudar o quê e onde.

### Como Funciona?
* **Monitoramento Contínuo:** O serviço monitora e registra continuamente as configurações dos seus recursos da AWS.
* **Avaliação com Regras:** Com o AWS Config, você pode automatizar a avaliação das configurações registradas em relação a um conjunto de regras que você define.
* **Visibilidade de Mudanças:** Você pode revisar as mudanças em sua configuração, as relações entre os recursos, e analisar históricos de configuração detalhados.

### Benefícios
Fazer essa análise simplifica a **auditoria de conformidade, a análise de segurança, o gerenciamento de mudanças e a solução de problemas operacionais**.

### Painel (Dashboard)
O painel do AWS Config mantém uma listagem de inventário de todos os recursos que existem na conta e, em seguida, verifica as regras de configuração.
* **Recursos não conformes são sinalizados**, alertando sobre problemas de configuração que você precisa resolver.

### Escopo do Serviço
* O Config é um **serviço regional**. Para rastrear recursos entre regiões, você precisa habilitá-lo em cada região que deseja usar.
* Ele também oferece um **recurso de agregador** que pode mostrar recursos de várias regiões e até de várias contas em uma única visualização.

---

## Ferramenta 2: AWS Artifact - Para Documentação e Acordos

### O que é?
O AWS Artifact fornece **downloads sob demanda de documentos de segurança e conformidade da AWS** (como relatórios de auditoria).

### Como Usar os Documentos?
* **Demonstrar Conformidade a Auditores:** Você pode enviar os documentos aos seus auditores para demonstrar a segurança e a conformidade da infraestrutura e dos serviços da AWS que você utiliza.
* **Diretrizes Internas:** Você pode usar esses documentos como guias para avaliar sua própria arquitetura na nuvem e a eficácia dos controles internos da sua empresa.

> **A Responsabilidade do Cliente:**
> O Artifact documenta a conformidade da AWS. Os clientes da AWS são responsáveis por desenvolver ou obter seus próprios documentos que demonstrem a segurança e a conformidade de **suas próprias aplicações**.

### Gerenciamento de Acordos
Você também pode usar o AWS Artifact para revisar, aceitar e rastrear o status de acordos da AWS.
* **Exemplo de Acordo:** O **Acordo de Associado de Negócios (Business Associate Agreement, ou BAA)**, que é tipicamente exigido por empresas sujeitas à HIPAA para garantir a proteção de informações de saúde.
* **Funcionalidade:** Com o AWS Artifact, você pode aceitar acordos com a AWS e designar contas da AWS que podem processar legalmente informações restritas.
* **Múltiplas Contas:** Para aceitar acordos em nome de várias contas, você pode usar o **AWS Organizations** para criar uma organização.

# Módulo 4: Revisão Final e Questão Prática

## Resumo dos Tópicos Aprendidos

Em resumo, ao concluir este módulo, você se tornou capaz de:

* **Reconhecer o modelo de responsabilidade compartilhada**, identificando a responsabilidade da AWS e a do cliente.
* **Reconhecer os componentes do IAM**: usuários, grupos e funções (roles).
* **Descrever os diferentes tipos de credenciais de segurança** no IAM.
* **Identificar os passos para proteger uma nova conta AWS**.
* **Proteger os dados da AWS** em trânsito e em repouso.
* **Descrever os programas de conformidade (compliance)** da AWS.

---

## Análise de Questão Prática (Exemplo de Exame)

### A Pergunta

> "Qual das seguintes opções é responsabilidade da AWS sob o modelo de Responsabilidade Compartilhada da AWS?"

### Análise das Palavras-Chave

* **"Responsabilidade da AWS":** É o foco da busca, o que você precisa encontrar na lista de opções.
* **"Modelo de Responsabilidade Compartilhada":** É o contexto, o conceito que define as regras para a resposta correta.

### A Resposta Correta

A resposta correta é **B, manter o hardware físico.**

# Guia de Segurança Avançada e em Escala na AWS

## 1. AWS Organizations: Gerenciamento Central de Contas

### O que é?
O AWS Organizations é um serviço de gerenciamento de contas que permite consolidar várias contas da AWS em uma organização que você cria e gerencia centralmente. Embora seja muito usado para faturamento consolidado, seu foco aqui são os recursos de segurança.

### Recurso Chave de Segurança: Políticas de Controle de Serviço (SCPs)
* **Agrupamento de Contas:** Você pode agrupar várias contas em **Unidades Organizacionais (OUs)**.
* **Aplicação de Políticas em Larga Escala:** É possível anexar diferentes políticas de acesso (SCPs) a cada OU. Isso funciona como uma maneira de aplicar permissões a múltiplas contas da AWS ao mesmo tempo, de forma análoga a como o IAM aplica políticas a grupos de usuários.
* **Estrutura Lógica:** Permite que você tenha contas separadas por departamento ou equipe, mas ainda represente sua empresa como uma única unidade lógica.
* **Expansão do Controle do IAM:** O Organizations expande o controle do IAM para o nível da conta, dando a você controle sobre o que usuários e funções em uma conta podem fazer.

### SCPs em Detalhe: As "Barreiras de Proteção"
As SCPs oferecem controle central sobre as **permissões máximas disponíveis** para todas as contas em sua organização, garantindo que elas permaneçam dentro das diretrizes de controle de acesso.

> **A REGRA MAIS IMPORTANTE:**
> As Políticas de Controle de Serviço (SCPs) **NUNCA CONCEDEM PERMISSÕES**. Em vez disso, elas são políticas em sintaxe JSON que especificam as permissões máximas, agindo como uma "barreira de proteção" (safeguard) para as ações que as contas podem realizar.

* **Relação com o IAM:** As SCPs não substituem a necessidade de políticas do IAM bem gerenciadas. Você **ainda deve anexar políticas do IAM** a usuários e funções dentro de cada conta para efetivamente conceder permissões a eles.
* **Pré-requisito:** As SCPs estão disponíveis apenas em uma organização que tenha **todos os recursos habilitados**, não apenas o recurso de faturamento consolidado.

---

## 2. AWS Key Management Service (KMS): Gerenciamento de Criptografia

### O que é?
O KMS é um serviço que permite criar e gerenciar chaves de criptografia e controlar o uso da criptografia em uma ampla gama de serviços da AWS e em suas aplicações.

### Como Funciona e Principais Recursos
* **Segurança de Hardware:** É um serviço seguro que utiliza **Módulos de Segurança de Hardware (HSMs)** para proteger suas chaves.
* **Auditoria:** Integra-se com o AWS CloudTrail para fornecer logs de todo o uso de chaves, ajudando a atender a necessidades de regulamentação e conformidade.
* **Hierarquia de Chaves:** As **Chaves Mestras do Cliente (CMKs)** são usadas para controlar o acesso a outras chaves que criptografam e descriptografam seus dados.
* **Gerenciamento Flexível:** Você pode criar novas chaves mestras, gerenciar quem tem acesso a elas, com quais serviços podem ser usadas e até importar chaves de sua própria infraestrutura de gerenciamento.
* **Ampla Integração:** O KMS se integra com a maioria dos serviços da AWS, permitindo que você use as chaves mestras para controlar a criptografia de dados armazenados nesses serviços.

---

## 3. Amazon Cognito: Identidade para Aplicações

### O que é?
O Amazon Cognito fornece soluções para controlar o acesso a recursos da AWS **a partir de sua aplicação**. Ele gerencia a identidade de usuários para seus aplicativos.

### Como Funciona?
* Você pode definir funções (roles) e mapear usuários para diferentes funções, garantindo que sua aplicação acesse apenas os itens autorizados para cada usuário.
* Utiliza padrões comuns de gerenciamento de identidade, como o **Security Assertion Markup Language (SAML) 2.0**.

### Benefício do SAML: Single Sign-On (SSO)
O SAML é um padrão aberto que permite a troca de informações de identidade e segurança. Com ele, você pode habilitar o **Single Sign-On (SSO)**, permitindo que seus usuários façam login em todas as suas aplicações habilitadas para SAML usando um único conjunto de credenciais corporativas (como do Microsoft Active Directory).

### Foco em Conformidade
O Cognito ajuda a atender a múltiplos requisitos de segurança e conformidade, incluindo aqueles de organizações altamente regulamentadas, como empresas de saúde e comerciantes.

---

## 4. AWS Shield: Proteção Contra Ataques DDoS

### O que é?
O AWS Shield é um serviço gerenciado de proteção contra ataques de **Negação de Serviço Distribuída (DDoS)** que protege as aplicações que rodam na AWS.

### Como Funciona?
* **Sempre Ativo:** Fornece detecção sempre ativa e mitigações automáticas que minimizam o tempo de inatividade e a latência da aplicação.
* **Não requer intervenção:** Não há necessidade de acionar o suporte da AWS para se beneficiar da proteção básica contra DDoS.

### Tipos de Ataques Protegidos
* **Camada de Infraestrutura:** Ex: Inundações UDP (User Datagram Protocol).
* **Ataques de Exaustão de Estado:** Ex: Inundações TCP SYN.
* **Camada de Aplicação:** Ex: Inundações HTTP GET ou POST.

### Níveis de Serviço (Tiers)

#### AWS Shield Standard
* **Custo:** Sem custo adicional.
* **Disponibilidade:** Habilitado automaticamente para **todos** os clientes da AWS.

#### AWS Shield Advanced
* **Custo:** É um serviço pago opcional.
* **Proteção:** Fornece proteção adicional contra ataques mais sofisticados e de maior volume.
* **Recursos Protegidos:** Aplica-se a recursos específicos como Amazon EC2, Elastic Load Balancers, Amazon CloudFront, Amazon Global Accelerator e Amazon Route 53.
* **Suporte Especializado:** Para contatar a equipe de resposta a DDoS (DDoS Response Team), os clientes precisam ter um plano de suporte **Business** ou **Enterprise**.

# Módulo 5: Redes e Entrega de Conteúdo

## Tópicos Abordados no Módulo
Este módulo está dividido em duas áreas principais:

### 1. Redes (Networking)
* Conceitos básicos de redes.
* Redes e segurança do Amazon VPC.

### 2. Entrega de Conteúdo (Content Delivery)
* Amazon Route 53.
* Amazon CloudFront.

---

## Recursos de Aprendizagem Disponíveis
* **Demonstração:** Mostrará como usar o Assistente VPC (VPC Wizard) para criar uma VPC com sub-redes pública e privada.
* **Laboratório Prático (Lab):** Onde você usará o assistente para construir uma VPC e lançar um servidor web.
* **Verificação de Conhecimento:** Para testar sua compreensão dos conceitos-chave.

---

## Objetivos de Aprendizagem
Ao final deste módulo, você será capaz de:
* Reconhecer os conceitos básicos de redes.
* Descrever os recursos do Amazon VPC e projetar uma arquitetura VPC básica.
* Entender o que são **Grupos de Segurança (Security Groups)** e **ACLs de Rede (Network ACLs)**.
* Identificar os fundamentos do Amazon Route 53.
* Reconhecer os benefícios do Amazon CloudFront.

# Guia de Conceitos Básicos de Redes

## O que é uma Rede de Computadores?
Uma rede de computadores é composta por duas ou mais máquinas conectadas para se comunicarem. Uma rede requer um dispositivo de rede, como um **roteador** ou um **switch**, que conecta todas as máquinas e permite a comunicação entre elas. Uma rede também pode ser logicamente particionada em **sub-redes**.

---

## Endereços IP: O "RG" de cada Máquina
Cada máquina em uma rede tem um **endereço de protocolo de internet (IP)** único atribuído a ela. Um endereço IP é um número único usado para identificar uma máquina de forma exclusiva, de forma semelhante a um número de telefone.

### 1. IPv4 (O Padrão Tradicional)
É a versão mais comum de endereços IP.
* **Formato:** Quatro números decimais separados por pontos.
    * Exemplo: `192.0.2.0`
* **Estrutura:** Cada um dos quatro números representa 8 bits, o que significa que cada número pode variar de **0 a 255**.
* **Tamanho Total:** A combinação dos quatro números resulta em um endereço de **32 bits**.

### 2. IPv6 (A Nova Geração)
Foi criado para compensar o esgotamento dos endereços IPv4, pois pode acomodar muito mais dispositivos.
* **Formato:** Oito grupos de quatro letras e números (hexadecimais) separados por dois-pontos.
* **Estrutura:** Cada um dos oito grupos representa 16 bits, podendo variar de `0` a `FFFF`.
* **Tamanho Total:** A combinação dos oito grupos resulta em um endereço de **128 bits**.

---

## Notação CIDR (Agrupando Endereços)

O **Classless Inter-Domain Routing (CIDR)** é um método comum para descrever redes e grupos de endereços IP consecutivos.

### Como Funciona?
O endereço é expresso como um endereço IP (que é o primeiro endereço da rede), seguido por uma barra (`/`) e um número.
* O número após a barra (ex: `/24`) informa quantos bits do endereço são fixos para o **identificador da rede** (o prefixo de roteamento).
* Os bits restantes ficam disponíveis para definir os endereços das máquinas individuais dentro daquela rede.

### Exemplo Prático
* **Endereço CIDR:** `192.0.2.0/24`
* **Análise:**
    * O `/24` significa que os primeiros 24 bits (`192.0.2`) são fixos e identificam a rede.
    * Os 8 bits restantes (32 bits totais - 24 bits fixos) podem variar.
    * Como 8 bits podem representar 256 valores (de 0 a 255), o último número do IP pode variar dentro desse intervalo.
* **Resultado:** Este bloco CIDR representa todos os endereços IP desde `192.0.2.0` até `192.0.2.255`.

---

## O Modelo OSI (As Camadas da Comunicação)

O modelo OSI é um modelo conceitual de sete camadas usado para explicar como os dados viajam por uma rede. Ele mostra os protocolos e endereços comuns usados em cada etapa.

### Exemplos de Camadas:
* **Camada 2 (Camada de Enlace de Dados):** Onde operam dispositivos como Hubs e Switches.
* **Camada 3 (Camada de Rede):** Onde operam os Roteadores.

O modelo OSI é útil para entender como a comunicação ocorre tanto em redes básicas quanto na nuvem.

# Guia de Conectividade e Roteamento na Amazon VPC

Este guia detalha os diferentes componentes e serviços que você pode usar para conectar sua VPC e rotear o tráfego.

---

## Parte 1: Conectando sua VPC à Internet

### 1. Gateway da Internet (Internet Gateway)
* **O que é?** Um componente de VPC escalável, redundante e altamente disponível que permite a comunicação entre instâncias em sua VPC e a internet pública.
* **Para que serve?**
    1.  Fornecer um alvo em suas tabelas de rotas da VPC para o tráfego da internet.
    2.  Realizar a Tradução de Endereços de Rede (NAT) para instâncias que receberam endereços IP públicos.
* **Como usar?** Para tornar uma sub-rede pública, você anexa um gateway da internet à sua VPC e adiciona uma entrada de rota à tabela de rotas associada à sub-rede.

### 2. Gateway NAT (NAT Gateway)
* **O que é?** Permite que instâncias em uma **sub-rede privada** se conectem à internet ou a outros serviços da AWS, mas **impede que a internet pública inicie uma conexão** com essas instâncias.
* **Como configurar?**
    1.  Você deve especificar a **sub-rede pública** na qual o gateway NAT deve residir.
    2.  Você deve especificar um **endereço IP Elástico** para associar ao gateway NAT.
    3.  Você deve atualizar a tabela de rotas da sua **sub-rede privada** para apontar o tráfego destinado à internet para o gateway NAT.
> **Recomendação da AWS:**
> Use um **Gateway NAT** em vez de uma **Instância NAT**. Um Gateway NAT é um serviço gerenciado que oferece melhor disponibilidade, maior largura de banda e menos esforço administrativo.

---

## Parte 2: Conectando Múltiplas VPCs e Contas

### 1. Compartilhamento de VPC (VPC Sharing)
* **O que é?** Permite que clientes compartilhem sub-redes com outras contas da AWS dentro da mesma Organização (AWS Organizations).
* **Como funciona?** A conta "proprietária" da VPC compartilha uma ou mais sub-redes com contas "participantes". Os participantes podem então visualizar, criar, modificar e excluir seus próprios recursos de aplicação (EC2, RDS, etc.) nessas sub-redes compartilhadas.

### 2. Conexão de Emparelhamento de VPC (VPC Peering)
* **O que é?** Permite que você roteie tráfego de forma privada entre duas VPCs, como se as instâncias estivessem na mesma rede.
* **Como funciona?** Você cria a conexão de emparelhamento e atualiza as tabelas de rotas em **ambas** as VPCs para que o destino do tráfego seja o intervalo de IP da outra VPC e o alvo seja o ID do recurso de emparelhamento.
* **Restrições Importantes:**
    1.  Os intervalos de endereços IP das VPCs **não podem se sobrepor**.
    2.  Só pode haver **uma** conexão de emparelhamento entre as mesmas duas VPCs.
    3.  **Emparelhamento transitivo não é suportado.** (Se a VPC-A está emparelhada com a VPC-B, e a VPC-B com a VPC-C, a VPC-A **não** pode se comunicar com a VPC-C através da B).

### 3. Gateway de Trânsito (Transit Gateway)
* **O Problema que Resolve:** A complexidade de conectar centenas de VPCs usando VPC Peering, que exigiria uma conexão dedicada para cada par.
* **O que é?** Um hub de trânsito de rede que você usa para interconectar suas VPCs e redes on-premises.
* **Como funciona?** Cria uma topologia "hub and spoke" (hub e raios), na qual você pode anexar VPCs, gateways do AWS Direct Connect ou conexões VPN.
* **Benefícios:** Reduz drasticamente o número de conexões necessárias, a complexidade de implementação e a manutenção.

---

## Parte 3: Conectando sua VPC a Redes Remotas (On-Premises)

### 1. VPN Site-to-Site e Gateway Privado Virtual
* **O Problema que Resolve:** Por padrão, instâncias na VPC não podem se comunicar com sua rede local/remota.
* **A Solução:** Para habilitar o acesso, você precisa:
    1.  Anexar um **Gateway Privado Virtual (Virtual Private Gateway)** à VPC.
    2.  Criar uma tabela de rotas personalizada.
    3.  Atualizar suas regras de grupo de segurança.
    4.  Criar uma conexão **VPN Site-to-Site da AWS**.
    5.  Configurar o roteamento para passar o tráfego para a conexão.

### 2. AWS Direct Connect
* **O Problema que Resolve:** Desempenho de rede ruim ou inconsistente quando seu data center está geograficamente distante da sua Região AWS.
* **O que é?** Permite estabelecer uma **conexão privada e dedicada** entre sua rede e um dos locais do Direct Connect.
* **Benefícios:** Aumenta a largura de banda, a taxa de transferência e fornece uma experiência de rede mais consistente do que conexões baseadas na internet ou VPN.
* **Tecnologia:** Usa o padrão aberto 802.1Q de VLANs.

---

## Parte 4: Conectando sua VPC a Serviços AWS (Privadamente)

### 1. Endpoints de VPC
* **O Problema que Resolve:** A necessidade de conectar recursos da VPC a serviços regionais da AWS (como S3 e DynamoDB) sem que o tráfego passe pela internet pública.
* **O que é?** Um dispositivo virtual que permite conectar privadamente sua VPC a serviços AWS suportados, mantendo o tráfego dentro da rede da Amazon.

#### Tipo A: Endpoint de Gateway
* É um gateway que você especifica como um alvo na sua tabela de rotas.
* Usado para tráfego destinado ao **Amazon S3** ou **Amazon DynamoDB**.

#### Tipo B: Endpoint de Interface (usando AWS PrivateLink)
* É uma solução mais recente que usa o **AWS PrivateLink**.
* Simplifica a segurança ao eliminar a exposição de dados à internet pública, fornecendo conectividade privada entre VPCs, serviços AWS e aplicações on-premises.
* Facilita a conexão de serviços entre diferentes contas e VPCs, simplificando significativamente a arquitetura de rede.

# Como Criar uma VPC com Sub-redes Pública e Privada (Usando o Assistente)

Este guia é um passo a passo baseado na demonstração de criação de uma VPC, mostrando como usar o assistente e explorar os componentes criados.

## Parte 1: Preparação e Conceitos Iniciais

### O que é uma VPC?
A Amazon Virtual Private Cloud (VPC) é a sua própria fatia privada e logicamente isolada da rede AWS. Você tem controle total sobre o ambiente, incluindo a seleção do intervalo de IPs, criação de sub-redes, configuração de tabelas de rotas e gateways de rede.

### A VPC Padrão
> **Atenção:** Toda conta AWS vem com uma **VPC Padrão** em cada região. Ela é pré-fabricada para facilitar testes e experimentação. Para ambientes de produção ou de negócios, é fortemente recomendado criar sua própria VPC customizada, definindo e documentando cada componente.

### Conceitos que Você Precisa Conhecer
* **CIDR (Classless Inter-Domain Routing):** A notação para especificar um bloco de endereços IP (ex: `10.0.0.0/16`).
* **Gateway da Internet:** O componente que conecta sua VPC à internet pública.
* **Rotas:** Regras que ditam como o tráfego deve fluir para dentro e fora das sub-redes.
* **Sub-redes:** Subdivisões da sua VPC para organizar recursos.

---

## Parte 2: O Passo a Passo da Criação

### Passo 1: Criar um Endereço IP Elástico (Pré-requisito)
**Por que isso é necessário?** O assistente VPC criará um **Gateway NAT** para permitir que recursos em sub-redes privadas acessem a internet. Todo Gateway NAT precisa de um endereço IP público e estático, que é um Endereço IP Elástico.

**Ação:**
1.  No Console da AWS, navegue até o serviço **VPC**.
2.  No menu à esquerda, clique em **Endereços IP Elásticos (Elastic IP addresses)**.
3.  Clique em **Alocar novo endereço** e, em seguida, em **Alocar**.
4.  Um novo IP Elástico será criado e listado.

### Passo 2: Utilizar o Assistente VPC (VPC Wizard)
**Ação: Encontrar o Assistente**
1.  No menu à esquerda do console da VPC, clique no item do topo: **Painel da VPC (VPC dashboard)**.
2.  Clique no botão **Lançar assistente VPC (Launch VPC wizard)**.

**Ação: Escolher um Modelo**
O assistente oferece vários modelos. O que usaremos é o de **VPC com sub-redes pública e privada**. Este modelo é ideal para separar recursos voltados para a internet (na sub-rede pública) de recursos de back-end (na sub-rede privada).

**Ação: Configurar a VPC**
1.  Selecione a opção **VPC com sub-redes pública e privada** e clique em **Selecionar**.
2.  Preencha os seguintes campos:
    * **Bloco CIDR IPv4 da VPC:** Pode manter o padrão (ex: `10.0.0.0/16`).
    * **Nome da VPC:** Dê um nome, por exemplo: `myVPC`.
    * **Bloco CIDR da sub-rede pública:** Defina um sub-bloco, por exemplo: `10.0.1.0/24`.
    * **Zona de Disponibilidade (AZ):** Escolha a primeira da lista (ex: `us-west-2a`).
    * **Nome da sub-rede pública:** Dê um nome, por exemplo: `public subnet 1`.
    * **Bloco CIDR da sub-rede privada:** Defina um sub-bloco diferente, por exemplo: `10.0.2.0/24`.
    * **Zona de Disponibilidade (AZ):** Mantenha a mesma da sub-rede pública.
    * **Nome da sub-rede privada:** Dê um nome, por exemplo: `private subnet 1`.
    * **IP Elástico para o Gateway NAT:** Selecione o IP Elástico que você criou no Passo 1.
3.  Deixe as outras opções como estão e clique em **Criar VPC**.

---

## Parte 3: Explorando e Verificando os Recursos Criados

Após o assistente concluir, é crucial entender o que foi criado.

### 1. Suas VPCs
* Navegue até **Suas VPCs**. Você verá a nova `myVPC` listada junto com a VPC padrão.
* Clicando nela, você pode ver detalhes como seu ID e o bloco CIDR principal.

### 2. Gateways da Internet
* Navegue até **Gateways da Internet**. Você verá um novo gateway anexado à `myVPC`. Este componente é essencial para a comunicação com a internet. Ele é horizontalmente escalado, redundante e altamente disponível, não impondo riscos de disponibilidade ou gargalos de banda.

### 3. Sub-redes
* Navegue até **Sub-redes**. Uma sub-rede é um segmento de uma VPC que existe em **uma única Zona de Disponibilidade**.
* Você verá a `public subnet 1` e a `private subnet 1`.

#### Análise da Sub-rede PÚBLICA (`public subnet 1`)
* Ao selecioná-la e clicar na aba **Tabela de Rotas**, você verá duas rotas principais:
    1.  **Destino `10.0.0.0/16` | Alvo `local`:** Esta é a rota local, permitindo que todos os recursos dentro da VPC se comuniquem entre si.
    2.  **Destino `0.0.0.0/0` | Alvo `igw-...`:** Esta rota envia todo o tráfego destinado à internet para o **Gateway da Internet**. É esta rota que **define** uma sub-rede como pública.

#### Análise da Sub-rede PRIVADA (`private subnet 1`)
* Ao selecioná-la e clicar na aba **Tabela de Rotas**, você também verá duas rotas principais:
    1.  **Destino `10.0.0.0/16` | Alvo `local`:** A mesma rota local para comunicação interna.
    2.  **Destino `0.0.0.0/0` | Alvo `nat-...`:** Esta rota envia todo o tráfego destinado à internet para o **Gateway NAT**. Isso cria uma "rua de mão única", permitindo que recursos na sub-rede privada acessem a internet (para atualizações, patches, etc.), mas impedindo que a internet inicie conexões com eles.

### 4. Listas de Controle de Acesso à Rede (Network ACLs)
* Uma Network ACL é uma camada opcional de segurança que atua como um **firewall para sub-redes**.
* O assistente cria uma NACL padrão para a `myVPC` que é **aberta**:
    * **Regra de Entrada 100:** Permite TODO o tráfego de entrada.
    * **Regra de Saída 100:** Permite TODO o tráfego de saída.
    * **Regra `*` (asterisco):** Nega qualquer tráfego que não corresponda a uma regra numerada.

### 5. Outros Componentes
* **Grupos de Segurança (Security Groups):** Atuam como outra camada de proteção, funcionando como um firewall para os **recursos individuais** (como instâncias EC2) dentro das sub-redes.
* **Tags:** As marcações (chave-valor) que você pode usar para identificar seus recursos.
* **Logs de Fluxo da VPC (VPC Flow Logs):** O mecanismo de registro que captura todo o tráfego que entra e sai de sua VPC.

# Guia de Firewalls na VPC: Security Groups vs. Network ACLs

Você pode construir a segurança em sua arquitetura de VPC de várias maneiras, para que tenha controle completo sobre o tráfego de entrada e saída. A seguir, vamos detalhar as duas principais opções de firewall da Amazon VPC.

---

## 1. Grupos de Segurança (Security Groups): O Firewall da Instância

Um Grupo de Segurança atua como um firewall virtual que controla o tráfego de entrada e saída de e para sua instância.

### Como Funcionam?
* **Nível de Atuação:** Atuam no **nível da instância**, especificamente na placa de interface de rede (ENI). Você pode atribuir cada instância em sua VPC a um conjunto diferente de grupos de segurança.
* **Estado (State):** São **Stateful (com estado)**.
    * Isso significa que nós só nos preocupamos em definir as regras de tráfego de **entrada**. Se o tráfego de entrada em uma porta é permitido, o tráfego de saída correspondente (a resposta) é automaticamente permitido, independentemente das regras de saída.
* **Regras Suportadas:** Suportam apenas regras de **permissão (`allow`)**. Não é possível criar regras de negação (`deny`).
* **Comportamento Padrão:** Por padrão, um grupo de segurança vem **totalmente fechado**. Ele nega todo o tráfego de entrada até que você adicione regras para permitir tráfego específico.
* **Avaliação das Regras:** **Todas as regras** são avaliadas antes que uma decisão seja tomada para permitir o tráfego.

---

## 2. Listas de Controle de Acesso à Rede (Network ACLs): O Firewall da Sub-rede

As Network ACLs funcionam como um firewall que controla o tráfego que entra e sai de uma ou mais sub-redes.

### Como Funcionam?
* **Nível de Atuação:** Atuam no **nível da sub-rede**.
* **Estado (State):** São **Stateless (sem estado)**.
    * Isso significa que nenhuma informação sobre uma solicitação é mantida. Portanto, você precisa configurar regras explícitas **tanto para o tráfego de entrada quanto para o de saída**. Permitir uma solicitação de entrada não libera automaticamente a resposta de saída; ela precisa de uma regra correspondente.
* **Regras Suportadas:** Suportam tanto regras de **permissão (`allow`)** quanto de **negação (`deny`)**.
* **Comportamento Padrão:** A Network ACL padrão que vem com a VPC é **totalmente aberta** (permite todo tráfego de entrada e saída). Se você criar uma NACL personalizada, ela começa **totalmente fechada** e você precisa adicionar regras.
* **Avaliação das Regras:** As regras são avaliadas em **ordem numérica**, da menor para a maior. Assim que uma regra corresponde ao tráfego, ela é aplicada imediatamente e as regras subsequentes são ignoradas.
* **Associação:** Cada sub-rede em sua VPC deve ser associada a uma Network ACL. Uma sub-rede só pode ser associada a uma NACL por vez, mas uma NACL pode ser associada a múltiplas sub-redes.

---

## Tabela Comparativa: Security Group vs. Network ACL

| Característica | Grupos de Segurança (Security Groups) | Listas de Controle de Acesso (Network ACLs) |
| :--- | :--- | :--- |
| **Nível de Atuação** | Nível da **Instância** (ENI) | Nível da **Sub-rede** |
| **Regras Suportadas**| Apenas regras de **`Allow`** (Permissão) | Regras de **`Allow`** (Permissão) e **`Deny`** (Negação) |
| **Estado** | **Stateful** (com estado) | **Stateless** (sem estado) |
| **Avaliação das Regras**| **Todas** as regras são avaliadas. | As regras são avaliadas em **ordem numérica** até encontrar uma correspondência. |

# Guia Completo do Amazon Route 53

## Parte 1: O que é o Amazon Route 53?

### O Conceito de DNS
A resolução de nomes é o processo de traduzir um nome (como `www.google.com`) para o endereço IP correspondente. O protocolo DNS, ou **Sistema de Nomes de Domínio**, funciona como uma lista telefônica da internet, onde os nomes são trocados pelos endereços IP das máquinas.

### O Serviço Amazon Route 53
O Amazon Route 53 é o serviço de DNS da AWS. Ele lhe dá a capacidade de:
* Registrar um nome de domínio (ex: `suaempresa.com`).
* Ter o serviço cuidando dos nomes e hosts (registros) relacionados a esse domínio.

O serviço é altamente disponível, escalável e totalmente compatível com endereços IPv4 e IPv6.

---

## Parte 2: As Políticas de Roteamento

As políticas de roteamento determinam como o Route 53 responde às consultas de DNS. Cada uma serve a um propósito diferente.

### 1. Roteamento Simples (Simple Routing)
* **O que é?** Permite que você configure registros DNS padrão, sem nenhuma lógica especial.
* **Caso de Uso Típico:** Direcionar o tráfego para um único recurso, como um servidor web para o seu site.

### 2. Roteamento Ponderado (Weighted Routing)
* **O que é?** Você atribui pesos (porcentagens) aos registros para especificar com que frequência diferentes respostas são servidas.
* **Caso de Uso Típico:** Testes A/B ou implantações *blue-green*. Por exemplo, você pode enviar 99% do tráfego para um sistema A (produção estável) e 1% para um sistema B (com novas modificações) para verificar seu funcionamento antes de liberar para todos.

### 3. Roteamento Baseado em Latência (Latency-based Routing)
* **O que é?** O Route 53 responde à consulta com o recurso que proporcionará o menor tempo de resposta (latência) para o usuário solicitante.
* **Detalhe Importante:** Nem sempre será o caminho geograficamente mais curto, mas sim o mais rápido em termos de performance de rede naquele momento.

### 4. Roteamento por Geolocalização (Geolocation Routing)
* **O que é?** Permite que você escolha os recursos que servirão seu tráfego com base na localização geográfica de seus usuários.
* **Casos de Uso Típicos:**
    * Localizar seu conteúdo (ex: apresentar o site no idioma do usuário).
    * Restringir a distribuição de conteúdo apenas para locais onde você tem direitos de distribuição.

### 5. Roteamento de Failover (Failover Routing)
* **O que é?** Ajuda a detectar uma interrupção (falha) do seu site e redireciona os usuários para um local alternativo que esteja operando corretamente.
* **Pré-requisito Crucial:** Requer a configuração de uma **Verificação de Saúde (Health Check)**. Se a verificação de saúde falhar no local primário, o Route 53 passa a distribuir o endereço do local secundário.

### 6. Roteamento de Múltiplos Valores (Multi-value Routing)
* **O que é?** Permite combinar qualquer uma das outras opções de roteamento em uma resposta que pode retornar múltiplos valores (ex: múltiplos endereços IP para um mesmo nome).

---

## Parte 3: Aprofundando no DNS Failover

O failover de DNS permite melhorar a disponibilidade de sua aplicação, configurando cenários de backup.

### O que é uma Verificação de Saúde (Health Check)?
É um monitoramento que o Route 53 realiza para verificar a saúde e o desempenho de seus recursos. Cada verificação de saúde pode monitorar:
* A saúde de um recurso específico (como um servidor web).
* O status de outras verificações de saúde.
* O status de um alarme do Amazon CloudWatch.

### Exemplo Prático de Arquitetura de Failover
Este é um cenário típico para uma aplicação web de múltiplas camadas:

1.  **A Arquitetura Principal:** O Route 53 direciona o tráfego para um **Elastic Load Balancer**, que por sua vez distribui o tráfego para uma frota de **instâncias EC2**.

2.  **A Configuração no Route 53:**
    * Você cria dois registros DNS para o mesmo host (ex: `www.suaempresa.com`) com a política de **Failover**.
    * **Registro Primário:** Aponta para o Load Balancer da sua aplicação principal.
    * **Registro Secundário:** Aponta para um local de backup, como uma página web estática hospedada em um **bucket do Amazon S3**.

3.  **Como Funciona:**
    * As **Verificações de Saúde (Health Checks)** do Route 53 monitoram constantemente o site primário (o Load Balancer).
    * Se a verificação de saúde falhar, o Route 53 automaticamente para de enviar tráfego para o registro primário.
    * O serviço então passa a responder às consultas com o registro secundário, direcionando os usuários para a página estática no S3, que pode alertá-los de que o serviço está sendo restaurado.

# Guia do Amazon CloudFront: A CDN da AWS

## O Desafio: Latência e a Distância na Internet

Um dos maiores desafios da comunicação de rede é o **desempenho**.
* **O Problema:** Quando um usuário acessa um site, a solicitação precisa viajar por várias redes até o **servidor de origem**, onde a versão original dos dados (imagens, músicas, vídeos) está armazenada. A distância física entre o usuário e este servidor afeta significativamente o desempenho e a experiência de uso.
* **A Causa:** A **latência da rede** varia dependendo da localização geográfica dos usuários.
* **A Solução:** Uma **Rede de Entrega de Conteúdo (Content Delivery Network - CDN)** é uma parte essencial para garantir uma experiência de usuário fluida e rápida.

---

## A Solução: Amazon CloudFront

### O que é?
O Amazon CloudFront é o serviço de CDN da AWS. É um serviço rápido de entrega de conteúdo que entrega dados de forma segura aos clientes com altas velocidades de transferência e fornece um ambiente amigável para desenvolvedores.

### Como o Conteúdo é Entregue?
O CloudFront entrega os arquivos (seu conteúdo) aos usuários através de uma **rede global de locais de borda (edge locations)**.

### O Modelo de Negócios da AWS
O CloudFront é diferente das soluções tradicionais de CDN porque você pode aproveitar a entrega de conteúdo de alto desempenho:
* Sem contratos negociados.
* Sem preços altos ou taxas mínimas.
* É uma oferta de autoatendimento com preços no modelo **pague-pelo-uso (pay-as-you-go)**.

---

## Como o CloudFront Funciona na Prática

O processo de entrega de conteúdo acelerada envolve o Route 53 e os locais de borda.

1.  **A Solicitação:** Um cliente faz uma solicitação para acessar seu conteúdo (ex: uma imagem no seu site).
2.  **A Tradução (Route 53):** O **Amazon Route 53** usa a geolocalização para descobrir onde o cliente está localizado no mundo.
3.  **O Roteamento:** O Route 53 responde à solicitação com o endereço IP do **local de borda (edge location)** do CloudFront que está geograficamente mais próximo daquele cliente.
4.  **A Busca (Cache Miss):** O CloudFront, nesse local de borda, verifica se já possui uma cópia do conteúdo solicitado. Se não tiver, ele busca os dados do **servidor de origem** (onde o arquivo original reside).
5.  **O Cache:** O CloudFront **copia (armazena em cache)** os dados no local de borda.
6.  **A Entrega:** Os dados são finalmente entregues ao cliente a partir do local de borda (que está perto dele), resultando em uma experiência de usuário muito mais rápida. Em futuras solicitações da mesma região, o conteúdo será entregue diretamente do cache, sem precisar buscar no servidor de origem novamente.

---

## O Gerenciamento do Cache

### O que Acontece com Dados Antigos?
À medida que os dados se tornam obsoletos (desatualizados ou "stale"), eles são removidos do cache no local de borda para dar espaço a novos conteúdos.

### Como Controlar a Expiração?
Você pode definir a expiração dos dados no cache usando um número de **Tempo de Vida (Time-to-Live - TTL)**. Este valor define por quanto tempo (em segundos) os dados armazenados no cache do CloudFront permanecerão válidos antes que o CloudFront precise verificar novamente com o servidor de origem se há uma versão mais recente.

# Módulo 5: Revisão Final e Questão Prática

## Checklist de Aprendizagem do Módulo

Ao concluir este módulo, você aprendeu a:

* Reconhecer os conceitos básicos de redes.
* Descrever a rede virtual na nuvem com o Amazon VPC.
* Projetar uma arquitetura VPC básica.
* Listar os passos para construir uma VPC.
* Identificar os grupos de segurança (security groups).
* Criar sua própria VPC.
* Descrever os fundamentos do Amazon Route 53.
* Explicar os benefícios do Amazon CloudFront como uma rede de distribuição de conteúdo.

---

## Análise de Questão Prática (Exemplo de Exame)

### A Pergunta

> "Qual serviço de rede da AWS permite que uma empresa crie uma rede virtual dentro da AWS?"

### Análise das Palavras-Chave

* **"Serviço de rede da AWS":** Esta frase restringe o escopo das opções, focando apenas em serviços da categoria de rede.
* **"Criar uma rede virtual":** Esta frase indica a principal funcionalidade que o serviço deve oferecer.

### Processo de Eliminação

Vamos analisar as opções de resposta e eliminá-las com base nas palavras-chave:

* **Opção A (AWS Config):** Podemos eliminar esta opção porque o AWS Config **não é um serviço de rede**, mas sim de auditoria e conformidade.
* **Opções B e C (Amazon Route 53 e AWS Direct Connect):** Também podemos eliminar estas opções. Embora ambos sejam serviços de rede, eles **não são o que você usaria para criar uma rede virtual**.
    * O **Amazon Route 53** é um serviço web de DNS.
    * O **AWS Direct Connect** fornece uma conexão de rede privada dedicada entre a AWS e um data center do cliente.

### A Resposta Correta

A resposta correta é **D, Amazon VPC**.

A Amazon VPC permite que você provisione uma seção logicamente isolada da nuvem AWS, onde você pode lançar recursos da AWS em uma rede virtual que você define.

# Módulo 6: Computação (Compute)

## Tópicos Abordados no Módulo
* Uma visão geral dos serviços de computação.
* Amazon EC2.
* Otimização de custos do Amazon EC2.
* Serviços de contêiner.
* Uma introdução ao AWS Lambda.
* Uma introdução ao AWS Elastic Beanstalk.

---

## Recursos de Aprendizagem Disponíveis
* **Demonstração Gravada do EC2:** Para visualizar o serviço em ação.
* **Laboratório Prático (Hands-on):** Para praticar o lançamento de uma instância EC2 a partir do Console de Gerenciamento da AWS.
* **Análise Comparativa:** Explorar as vantagens e desvantagens de rodar um banco de dados no Amazon EC2 versus no Amazon RDS.
* **Atividades Adicionais:** Onde você explorará o AWS Lambda e o Elastic Beanstalk.
* **Verificação de Conhecimento:** Para testar sua compreensão dos conceitos-chave abordados.

---

## Objetivos de Aprendizagem
Ao final deste módulo, você será capaz de:
* Fornecer uma visão geral dos diferentes serviços de computação da AWS na nuvem.
* Demonstrar quando usar o Amazon Elastic Compute Cloud (Amazon EC2).
* Identificar a funcionalidade no console do EC2.
* Realizar funções básicas no Amazon EC2 para construir um ambiente de computação virtual.
* Identificar os elementos de otimização de custos do Amazon EC2.
* Demonstrar quando usar o AWS Elastic Beanstalk.
* Demonstrar quando usar o AWS Lambda.
* Identificar como executar aplicações em contêineres em um cluster de servidores gerenciados.

# Guia de Serviços de Computação (Compute) na AWS

## O Ecossistema de Computação da AWS (Visão Geral Rápida)

A AWS oferece muitos serviços de computação. Aqui está um breve resumo de cada um:

* **Amazon Elastic Compute Cloud (Amazon EC2):** Fornece máquinas virtuais redimensionáveis.
* **Amazon EC2 Auto Scaling:** Suporta a disponibilidade de aplicações, permitindo que você defina condições que lançarão ou terminarão automaticamente instâncias EC2.
* **Amazon Elastic Container Registry (Amazon ECR):** É usado para armazenar e recuperar imagens Docker.
* **Amazon Elastic Container Service (Amazon ECS):** É um serviço de orquestração de contêineres que suporta Docker.
* **VMware Cloud on AWS:** Permite que você provisione uma nuvem híbrida sem hardware personalizado.
* **AWS Elastic Beanstalk:** Fornece uma maneira simples de executar e gerenciar aplicações web.
* **AWS Lambda:** É uma solução de computação sem servidor (serverless). Você paga apenas pelo tempo de computação que usa.
* **Amazon Elastic Kubernetes Service (Amazon EKS):** Permite que você execute Kubernetes gerenciado na AWS.
* **Amazon LightSail:** Fornece um serviço simples de usar para construir uma aplicação ou um site.
* **AWS Batch:** Fornece uma ferramenta para executar trabalhos em lote (batch jobs) em qualquer escala.
* **AWS Fargate:** Fornece uma maneira de executar contêineres que reduz a necessidade de você gerenciar servidores ou clusters.
* **AWS Outposts:** Fornece uma maneira de executar serviços selecionados da AWS em seu data center local (on-premises).
* **AWS Serverless Application Repository:** Fornece uma maneira de descobrir, implantar e publicar aplicações sem servidor.

### Categorização de serviço computacional

| Serviços | Principais conceitos | Características | Facilidade de uso |
| :--- | :--- | :--- | :--- |
| **Amazon EC2** | • Infraestrutura como um serviço (IaaS)<br>• Baseado em instância<br>• Máquinas virtuais | • Provisone máquinas virtuais que você possa gerenciar como quiser. | Um conceito familiar para muitos profissionais de TI. |
| **AWS Lambda** | • Computação sem servidor<br>• Baseado em função<br>• Baixo custo | • Escrever e implantar código que seja executado por agendamento ou que possa ser acionado por eventos.<br>• Usar quando possível (arquitetar para a nuvem). | Um conceito relativamente novo para muitos membros da equipe de TI, mas fácil de usar depois de aprender como. |
| **Amazon ECS**<br>**Amazon EKS**<br>**AWS Fargate**<br>**Amazon ECR** | • Computação baseada em contêineres<br>• Baseado em instância | • Gerar e executar trabalhos com mais rapidez. | O AWS Fargate reduz a sobrecarga administrativa, mas você pode usar opções que oferecem mais controle. |
| **AWS Elastic Beanstalk** | • Plataforma como serviço (PaaS)<br>• Para aplicativos Web | • Concentre-se no código (criação do aplicativo).<br>• Pode ser facilmente vinculado a outros serviços—bancos de dados, DNS, etc. | Rápido e fácil de começar a usar. |

---

## As 4 Grandes Categorias de Serviços de Computação

Você pode pensar em cada serviço de computação da AWS como pertencente a uma de quatro categorias amplas.

### 1. Infraestrutura como Serviço (IaaS) - Máquinas Virtuais
* **Serviço Principal:** **Amazon EC2**.
* **Características:**
    * Oferece máxima **flexibilidade** e deixa muitas das responsabilidades de gerenciamento do servidor para você.
    * Você escolhe o sistema operacional, o tamanho e as capacidades de recursos dos servidores que lança.
    * Foi um dos primeiros serviços da AWS e continua sendo um dos mais populares.

### 2. Computação Sem Servidor (Serverless)
* **Serviço Principal:** **AWS Lambda**.
* **Características:**
    * É uma plataforma de computação de **administração zero**.
    * Permite que você execute código **sem provisionar ou gerenciar servidores**.
    * Você paga apenas pelo tempo de computação que é consumido.
    * Está se tornando mais popular porque suporta **arquiteturas nativas da nuvem**, que permitem escalabilidade massiva a um custo menor.

### 3. Computação Baseada em Contêineres
* **Serviços Principais:** **Amazon ECS**, **Amazon EKS**, **AWS Fargate**, **Amazon ECR**.
* **Características:**
    * Contêineres são provisionados **mais rapidamente** do que máquinas virtuais, devido à abstração do sistema operacional do processo de provisionamento.
    * As soluções baseadas em contêineres continuam a crescer em popularidade.

### 4. Plataforma como Serviço (PaaS) - Aplicações Web
* **Serviço Principal:** **AWS Elastic Beanstalk**.
* **Características:**
    * Facilita a **implantação rápida**, fornecendo todos os serviços de aplicação que você precisa.
    * A AWS gerencia o SO, o servidor de aplicação e outros componentes de infraestrutura.
    * Permite que você **se concentre no desenvolvimento do seu código** de aplicação.

---

## Como Escolher o Serviço de Computação Certo?

O serviço de computação ideal que você usará depende do seu caso de uso. Ao selecionar, você deve considerar as seguintes perguntas:

1.  **Qual é o design da sua aplicação?**
2.  **Quais são seus padrões de uso?**
3.  **Quais configurações você vai querer gerenciar?**

Selecionar a solução de computação errada para uma arquitetura pode levar a problemas de desempenho, disponibilidade ou implantação.

### O Processo de Decisão
* Você pode começar com um "melhor palpite" ou com base nas recomendações dos desenvolvedores para uma aplicação existente.
* Você também pode usar métricas e coletar dados relacionados à computação para reavaliar as necessidades com base no que os dados lhe dizem.
* Um cliente pode começar com uma solução e decidir mudar o design com base nos padrões de uso ou em mudanças na arquitetura da aplicação.

# Guia Fundamental do Amazon EC2: AMIs e Tipos de Instância

## Parte 1: O Problema On-Premises e a Solução EC2

### O Desafio dos Servidores Locais (On-Premises)
* **Custo Elevado:** Servidores precisam ser comprados e data centers precisam ser construídos, equipados com pessoal e mantidos.
* **Provisionamento para Picos:** As organizações precisam comprar hardware suficiente para lidar com as cargas de trabalho de pico, o que resulta em capacidade ociosa e desperdício na maior parte do tempo.

### A Solução: Amazon Elastic Compute Cloud (EC2)
O Amazon EC2 é uma opção diferente que fornece **máquinas virtuais (VMs)** seguras e redimensionáveis na nuvem, onde você pode hospedar as mesmas aplicações que executa em servidores locais.

**Usos Comuns:** Servidores de aplicação, servidores web, servidores de banco de dados e muitos outros.

## Parte 2: O que é uma Instância EC2?
As VMs na nuvem da AWS são chamadas de **instâncias EC2**.
* **Controle Total:** Você tem controle administrativo total sobre o sistema operacional (Windows ou Linux) que roda nelas. A maioria dos SOs de servidor é suportada (Windows, Red Hat, SUSE, Ubuntu, Amazon Linux, etc.).
* **Escala e Agilidade:** Você pode lançar qualquer número de instâncias, de qualquer tamanho, em qualquer Zona de Disponibilidade no mundo inteiro, em questão de minutos.
* **Base de Lançamento:** As instâncias são lançadas a partir de **Imagens de Máquina da Amazon (AMIs)**.
* **Segurança:** O tráfego de e para as instâncias é controlado por **Grupos de Segurança (Security Groups)**.

## Parte 3: O Processo de Lançamento (Launch Instance Wizard)
A primeira vez que você lança uma instância, provavelmente usará o **Assistente de Lançamento de Instância** do Console AWS, que simplifica o processo. Embora seja possível aceitar os padrões, para a maioria das implantações, você modificará as configurações para atender às suas necessidades específicas.

---

## Parte 4: Decisão-Chave 1 - Imagens de Máquina da Amazon (AMIs)
A primeira decisão ao lançar uma instância é escolher a AMI. Pense nela como um **modelo** ou "molde".

* **Conteúdo:** Uma AMI contém um sistema operacional (Windows ou Linux) e, frequentemente, software adicional pré-instalado.
* **Uso:** Você pode usar AMIs diferentes para propósitos diferentes (ex: uma para um servidor web, outra para um servidor de aplicação) ou lançar múltiplas instâncias a partir de uma única AMI.

### As 4 Categorias de AMIs
1.  **Quick Start (Início Rápido):** AMIs pré-construídas e mantidas pela AWS.
2.  **Minhas AMIs (My AMIs):** AMIs que você mesmo criou.
3.  **AWS Marketplace:** Um catálogo com milhares de soluções de software de terceiros, prontas para usar.
4.  **AMIs da Comunidade:** AMIs compartilhadas por outros usuários.
    > **Atenção:** Estas AMIs não são verificadas pela AWS. Use-as por sua conta e risco e evite-as em qualquer ambiente de produção ou corporativo.

### Como Criar sua Própria AMI
1.  **Passo 1: Iniciar com uma Instância.**
    * Lance uma instância a partir de uma AMI existente (Quick Start, Marketplace, etc.) ou de uma VM que você importou do seu ambiente on-premises.
2.  **Passo 2: Modificar a Instância.**
    * Conecte-se à instância e personalize-a: instale patches de segurança, atualize o SO, instale softwares e bibliotecas (Python, Java, etc.). O resultado é uma "instância modificada".
3.  **Passo 3: Capturar a Nova AMI (na mesma região).**
    * A partir da sua instância modificada, você pode criar uma nova AMI. O EC2 irá parar a instância, criar um **snapshot** (uma cópia) do seu volume raiz e registrar esse snapshot como uma nova AMI.
    * Esta nova AMI pode ser usada para lançar novas instâncias idênticas na **mesma Região AWS**.
4.  **Passo 4: Copiar a AMI (para outras regiões).**
    * Se precisar lançar instâncias em outras regiões, você pode copiar sua AMI personalizada para essas localidades.

---

## Parte 5: Decisão-Chave 2 - Tipos de Instância
Após escolher a AMI ("o software"), você precisa escolher o **Tipo de Instância** ("o hardware").

* **O que é?** Tipos de instância são combinações pré-definidas de **CPU, memória, armazenamento e capacidade de rede**. Eles oferecem flexibilidade para escolher a mistura de recursos mais apropriada para sua aplicação.

### As Categorias de Tipos de Instância
* Uso Geral (General Purpose)
* Otimizada para Computação (Compute Optimized)
* Otimizada para Memória (Memory Optimized)
* Otimizada para Armazenamento (Storage Optimized)
* Instâncias de Computação Acelerada (Accelerated Computing)

### Como "Ler" um Nome de Instância (Ex: `T3.Large`)
* **`T`**: É a **família** da instância.
* **`3`**: É a **geração** da família. Gerações mais altas são geralmente mais poderosas e com melhor custo-benefício.
* **`Large`**: É o **tamanho** da instância. O tamanho geralmente dobra os recursos. Por exemplo, uma `T3.2XLarge` tem o dobro de CPUs e memória de uma `T3.XLarge`.

### Exemplos de Famílias e Casos de Uso
* **Família T3 (Uso Geral):** Fornece uma performance de CPU base com a capacidade de ter picos (*burst*). Ideal para aplicações web, ambientes de desenvolvimento, microserviços, etc.
* **Família C5 (Otimizada para Computação):** Para cargas de trabalho intensivas em CPU. Ideal para modelagem científica, processamento em lote, servidores de jogos, etc.
* **Família R5 (Otimizada para Memória):** Para aplicações que precisam de muita RAM. Ideal para bancos de dados de alta performance, bancos de dados em memória, análise de big data, etc.

## Parte 6: Otimização de Performance de Rede

* **Largura de Banda:** Cada tipo de instância tem um nível de desempenho de rede documentado (ex: até 10 Gbps vs. até 100 Gbps). É crucial escolher um tipo que atenda aos seus requisitos.
* **Grupos de Posicionamento (Placement Groups):** Permitem influenciar a localização física das instâncias para otimizar a performance da rede entre elas (ex: garantir baixa latência).
* **Rede Otimizada (Enhanced Networking):** Um recurso disponível em muitos tipos de instância para obter maior performance de pacotes por segundo, menor *jitter* e latências mais baixas.

# Guia Fundamental do Amazon EC2 (Parte 2): Rede, IAM, User Data e Armazenamento

Depois de escolher uma AMI e um Tipo de Instância (Parte 1), você deve tomar as seguintes decisões ao lançar uma instância EC2.

---

## Decisão 3: Configurações de Rede

Você deve especificar a localização de rede onde a instância EC2 será implantada.

* **Região:** A escolha da Região deve ser feita **antes** de você iniciar o Assistente de Lançamento de Instância.
* **VPC e Sub-rede:** Dentro da região, você pode colocar a instância em qualquer VPC e sub-rede existentes. O assistente também permite criar novas VPCs ou sub-redes, se necessário.

### Comportamento do IP Público
* **Ao lançar em uma VPC Padrão:** Por padrão, a AWS atribui um endereço IP público à instância.
* **Ao lançar em uma VPC Não Padrão:** A atribuição de um IP público depende de um atributo da sub-rede, mas você pode sobrescrever essa configuração durante o lançamento da instância.

---

## Decisão 4: Anexando uma Função (Role) do IAM

É comum usar instâncias EC2 para executar uma aplicação que precisa fazer chamadas de API para outros serviços da AWS.

> **PRÁTICA INCORRETA (A SER EVITADA):**
> Você **NUNCA deve armazenar credenciais da AWS (chaves de acesso) em uma instância EC2.** Não é seguro.

### A Solução Correta
A maneira segura de conceder permissões a uma aplicação rodando no EC2 é **anexar uma Função (Role) do IAM** à instância.
* **Perfil de Instância (Instance Profile):** É um contêiner para uma função do IAM. Ao criar uma role para o EC2 pelo console, um perfil de instância com o mesmo nome é criado automaticamente.
* **Flexibilidade:** Você pode anexar uma função do IAM tanto no momento do lançamento da instância quanto a uma instância já em execução.

---

## Decisão 5: Scripts de Dados do Usuário (User Data)

### O que é?
Ao criar uma instância EC2, você tem a opção de passar "dados do usuário". Estes são scripts que podem **automatizar a conclusão de instalações e configurações no primeiro lançamento da instância**.

### Casos de Uso
* Aplicar patches e atualizar o sistema operacional.
* Buscar e instalar softwares e chaves de licença.
* Instalar softwares adicionais (ex: `wget`).

### Como Escrever os Scripts
* **Para Linux:** Scripts de shell Bash.
    ```bash
    #!/bin/bash
    yum update -y
    yum install -y wget
    ```
* **Para Windows:** Scripts compatíveis com o prompt de comando, comandos de lote ou Windows PowerShell.

### Quando Roda?
O script de dados do usuário é executado durante as fases finais do processo de inicialização (boot) e, por padrão, **apenas na primeira vez** que uma instância é iniciada.

### Uso Estratégico
Os scripts de dados do usuário podem ser usados para **reduzir o número de AMIs personalizadas** que você precisa construir e manter. Em vez de manter softwares e configurações nas AMIs, você pode usar scripts separados para realizar essas ações no momento do lançamento.

---

## Decisão 6: Opções de Armazenamento

Ao lançar uma instância EC2, você pode configurar o armazenamento, incluindo o tamanho do volume raiz (onde o SO é instalado) e anexar volumes adicionais.

### Opções de Armazenamento em Bloco

#### 1. Amazon Elastic Block Store (EBS)
* **Definição:** Um serviço de armazenamento em bloco **durável**, de alto desempenho e fácil de usar.
* **Característica Chave:** Se você parar uma instância com volumes EBS e iniciá-la novamente, **os dados ainda estarão lá**.

#### 2. EC2 Instance Store
* **Definição:** Fornece armazenamento em bloco **temporário** para sua instância.
* **Localização:** Discos rígidos fisicamente conectados ao computador host.
* **Caso de Uso:** Ideal para armazenar temporariamente informações que mudam com frequência, como buffers e caches.
> **ALERTA CRÍTICO:**
> Os dados no Instance Store **SÃO PERMANENTEMENTE EXCLUÍDOS** se a instância for parada, terminada ou sofrer uma falha de hardware.

### Outras Opções de Armazenamento (Não-Raiz)
* **Amazon Elastic File System (EFS):** Fornece um sistema de arquivos de rede elástico, gerenciado e escalável.
* **Amazon S3:** É um serviço de armazenamento de objetos.

### Cenários Práticos e Comparação

#### Cenário 1: Instância com Raiz em EBS (EBS-backed)
* Se esta instância for parada e depois iniciada novamente, o volume do SO e qualquer dado armazenado nos volumes EBS **permanecerão intactos**.
* No entanto, qualquer dado que foi armazenado no volume de Instance Store (efêmero) **será permanentemente perdido**.

#### Cenário 2: Instância com Raiz em Instance Store (Instance Store-backed)
* Uma instância com um volume raiz de Instance Store **não pode ser parada** pela API do EC2; ela só pode ser **terminada**.
* Se a instância for terminada (ou falhar), **todos os dados no volume raiz serão perdidos**, incluindo o sistema operacional. Você não conseguirá iniciar essa instância novamente.

> **Recomendação Final:**
> **Não confie no Instance Store para dados valiosos e de longo prazo.** Em vez disso, use um armazenamento de dados mais durável como Amazon EBS, Amazon EFS ou Amazon S3.
> *(Nota: Se uma instância apenas **reiniciar (reboot)**, os dados no Instance Store permanecem disponíveis.)*

# Guia Fundamental do Amazon EC2 (Parte 3): Gerenciamento e Operação

## 1. Tags: Organizando seus Recursos
* **O que são?** Uma tag é um rótulo (uma chave e um valor opcional) que você atribui a um recurso da AWS.
* **Para que servem?** Permitem categorizar recursos de diferentes maneiras, como por propósito, proprietário ou ambiente. É a forma de anexar metadados a uma instância EC2.
* **Exemplo Comum:** A chave de tag `Name` com um valor descritivo, como `webserver1`. Esta tag é exibida por padrão no console do EC2.
* **Boa Prática:** Desenvolver uma estratégia de etiquetagem consistente para facilitar o gerenciamento de seus recursos.

## 2. Grupos de Segurança (Security Groups): Detalhes da Configuração
* **O que são?** Um firewall virtual que controla o tráfego de rede para uma ou mais instâncias. Se nenhum for especificado, o grupo de segurança padrão é usado.
* **Regras:** Você adiciona regras para permitir o tráfego. Todas as regras de todos os grupos de segurança associados a uma instância são avaliadas.
* **Origem/Destino das Regras:** Podem especificar:
    * Um endereço IP ou um intervalo de IPs.
    * Outro grupo de segurança.
    * Um endpoint de VPC.
    * "Qualquer lugar" (`0.0.0.0/0`).
* **Regra de Saída Padrão:** Por padrão, um grupo de segurança inclui uma regra que permite todo o tráfego de saída.

## 3. Pares de Chaves (Key Pairs): Conexão Segura
* **O que são?** Um par de chaves consiste em uma **chave pública** (que a AWS armazena) e uma **chave privada** (que você armazena) para permitir conexões seguras.
* **Momento da Decisão:** É uma escolha importante no final do assistente de lançamento: usar um par de chaves existente, criar um novo ou prosseguir sem um.
> **ALERTA CRÍTICO:**
> A única oportunidade que você tem para baixar e salvar a **chave privada** é no momento da sua criação. Guarde-a em um local seguro.

### Como Usar as Chaves
* **Conexão em Instâncias Windows (via RDP):** Você usa a chave privada para obter a senha de administrador e, em seguida, faz login usando o Protocolo de Área de Trabalho Remota (RDP).
* **Conexão em Instâncias Linux (via SSH):** Você deve fornecer a chave privada ao cliente SSH (como o PuTTY) para estabelecer a conexão.

## 4. Acessando e Gerenciando Instâncias

### Visualizando a Instância no Console
Após o lançamento, o painel de descrição exibe muitas informações úteis, como endereços IP, nomes DNS, ID da instância, ID da AMI, ID da VPC, ID da sub-rede e muito mais.

### Acessando Programaticamente com a AWS CLI
Você pode lançar instâncias usando a Interface de Linha de Comando da AWS. O comando principal é `aws ec2 run-instances` e requer vários parâmetros:
* `--image-id`: O ID da AMI a ser usada.
* `--count`: O número de instâncias a serem lançadas.
* `--instance-type`: O tipo de instância (ex: `c3.large`).
* `--key-name`: O nome do par de chaves a ser usado.
* `--security-groups`: O grupo de segurança a ser associado.
* `--region`: A região onde a AMI e outros recursos se encontram.

Para o comando ter sucesso, ele deve estar bem formado, os recursos referenciados devem existir, você deve ter as permissões necessárias e haver capacidade suficiente na conta.

## 5. O Ciclo de Vida da Instância (Instance Lifecycle)
As instâncias passam por diferentes estados ao longo de sua vida.

* **Pendente (Pending):** Estado inicial ao ser lançada ou iniciada após uma parada.
* **Em Execução (Running):** Estado normal, totalmente inicializada e pronta para acesso.
* **Reinicializando (Rebooting):** Uma instância em execução pode ser reinicializada.
    * Permanece no mesmo host físico.
    * Mantém o mesmo nome DNS público e IP público.
    * **Mantém os dados em volumes de Instance Store**.
* **Parando (Stopping) / Parada (Stopped):**
    * Aplicável **apenas a instâncias com volume raiz em Amazon EBS**.
    * A instância não incorre nos mesmos custos de uma em execução.
    * Ao ser iniciada novamente, ela é movida para uma **nova máquina host**.
* **Desligando (Shutting-down) / Terminada (Terminated):**
    * A instância é efetivamente excluída.
    * **Você não pode se conectar ou recuperar uma instância terminada.**

## 6. Endereços IP: Público vs. Elástico

* **Endereço IP Público (Dinâmico):** É um endereço IPv4 alcançável pela internet. Este IP é **liberado** quando a instância é **parada** ou **terminada**. Ao ser iniciada novamente, a instância recebe um **novo** endereço IP público.
* **Endereço IP Elástico (EIP):** Se você precisa de um IP público **persistente**, deve usar um IP Elástico. Você o aloca em sua conta e o associa à sua instância. Existe um limite flexível de 5 EIPs por região por conta.

## 7. Metadados da Instância (Instance Metadata)
* **O que são?** São dados *sobre* sua instância, que podem ser acessados *de dentro* dela.
* **Como Acessar:** Usando o endereço link-local `169.254.169.254/latest/metadata` em um navegador ou via linha de comando (com a ferramenta `curl`).
* **Quais Dados Estão Disponíveis?** IP público, IP privado, hostname, ID da instância, grupo de segurança, região, dados do usuário (user data) e muito mais.

## 8. Monitoramento com Amazon CloudWatch
* **O que é?** O CloudWatch coleta e processa métricas quase em tempo real de suas instâncias EC2, com estatísticas mantidas por 15 meses.
* **Níveis de Monitoramento:**
    * **Monitoramento Básico (padrão):** Envia dados de métricas para o CloudWatch a cada **5 minutos**.
    * **Monitoramento Detalhado (opcional):** Envia métricas a cada **1 minuto**.

# Como Lançar, Conectar e Terminar uma Instância EC2 (Guia Prático)

Este guia é um passo a passo baseado na demonstração de lançamento de uma instância Linux no Console de Gerenciamento da AWS.

## Preparação: Antes de Começar
1.  **Verifique a Região:** No canto superior direito do Console de Gerenciamento, certifique-se de que a região selecionada é a correta para o lançamento da sua instância.
2.  **Acesse o Serviço EC2:** Na barra de busca, digite `EC2` e selecione o serviço.

---

## Parte 1: Lançando a Instância EC2 (Usando o Assistente)

### Passo 1: Iniciar o Assistente
* No **Painel do EC2** ou na página **Instâncias**, clique no botão laranja **Lançar Instância**.

### Passo 2: Nome e Tags
* No campo **Nome**, dê um nome descritivo para sua instância (ex: `Academy Demo`).
* *Nota: Isso cria automaticamente uma Tag com a chave `Name` e o valor que você inseriu.*

### Passo 3: Imagem da Aplicação e SO (AMI)
* Na seção **"Imagens de aplicação e SO"**, escolha um "molde" para sua instância.
* Na aba **Quick Start**, selecione a AMI desejada (ex: `Amazon Linux 2 AMI`).
* *Nota: Você também pode usar suas próprias AMIs ("Minhas AMIs") ou AMIs do "Marketplace".*

### Passo 4: Tipo de Instância
* Na seção **"Tipo de Instância"**, selecione as especificações de hardware (CPU, memória).
* Use a lista suspensa para escolher o tipo (ex: `t2.micro`, que está no nível gratuito).

### Passo 5: Par de Chaves (Key Pair) para Login
* Na seção **"Par de chaves (login)"**, selecione a chave que será usada para acessar a instância via SSH.
* **Se você já tem uma chave:** Selecione-a na lista. Certifique-se de ter o arquivo `.pem` correspondente.
* **Se você não tem uma chave:** Clique em **Criar um novo par de chaves**, dê um nome, e **faça o download do arquivo `.pem` imediatamente**. Guarde-o em um local seguro.
* *Nota: Não é recomendado prosseguir sem um par de chaves se você pretende acessar a instância.*

### Passo 6: Configurações de Rede
* Na seção **"Configurações de Rede"**, clique em **Editar**.
* **VPC:** Selecione a VPC onde a instância será lançada.
* **Sub-rede:** Selecione uma sub-rede. Para este guia, escolha uma **sub-rede pública**.
* **Atribuir IP público automaticamente:** Deixe como **Habilitar** para que a instância seja acessível pela internet.

### Passo 7: Firewall (Grupos de Segurança)
* Na mesma seção de rede, configure o firewall.
* **Opção 1 (Recomendado):** Escolha **Selecionar grupo de segurança existente** e selecione um grupo que já tenha as regras de que você precisa (ex: um que permita tráfego SSH e HTTPS).
* **Opção 2:** Deixe **Criar um novo grupo de segurança** selecionado, dê um nome e adicione as regras de entrada necessárias.

### Passo 8: Configurar Armazenamento
* Na seção **"Configurar armazenamento"**, você pode ajustar o tamanho e o tipo do volume raiz (onde o SO é instalado). Para este guia, as configurações padrão são suficientes.

### Passo 9: Detalhes Avançados (Opcional)
* Expanda a seção **"Detalhes avançados"** para ver outras opções, como:
    * **Solicitar Instâncias Spot:** Para usar o modelo de preço Spot.
    * **Perfil da instância IAM:** Para anexar uma Role do IAM à instância.
    * **Proteção contra terminação/parada:** Para evitar ações acidentais.
    * **Dados do usuário:** Para inserir um script que roda na primeira inicialização da instância.

### Passo 10: Lançar e Verificar
1.  No painel **Resumo** à direita, verifique suas configurações.
2.  Clique em **Lançar Instância**.
3.  Após a mensagem de "Sucesso", clique em **Ver todas as instâncias**.
4.  Observe a sua nova instância. O **Status da instância** mudará de `Pendente` para `Em execução`, e a **Verificação de status** eventualmente mostrará "2/2 verificações aprovadas".

---

## Parte 2: Conectando-se à Instância (Linux)

### Método 1: Conexão via SSH (Usando o PuTTY)
1.  **Obter o Endereço IP:** Selecione sua instância na lista e, no painel de detalhes abaixo, copie o **Endereço IP público IPv4**.
2.  **Configurar o PuTTY:**
    * Cole o endereço IP no campo "Host Name (or IP address)".
    * No menu à esquerda, navegue até `Connection` > `SSH` > `Auth`.
    * Clique em `Browse...` e selecione seu arquivo de chave privada.
    * (Opcional) Em `Connection`, defina um valor em "Seconds between keepalives" (ex: `60`) para manter a sessão ativa.
3.  **Conectar:**
    * Clique em **Open**.
    * Na primeira conexão, aceite o alerta de segurança do host.
    * No prompt de login, digite o nome de usuário padrão para a AMI (para Amazon Linux, é `ec2-user`).
    * Parabéns, você está conectado!

### Método 2: Conexão via EC2 Instance Connect (No Console)
1.  **Acessar a Ferramenta:** Selecione a instância na lista e clique no botão **Conectar** no topo da página.
2.  **Conectar:** Na aba **EC2 Instance Connect**, o nome de usuário já estará preenchido. Apenas clique em **Conectar**.
3.  **Resultado:** Uma janela de terminal abrirá no seu navegador, já logada na instância. Para desconectar, basta fechar a aba.

---

## Parte 3: Terminando (Excluindo) a Instância
1.  Selecione a instância que deseja excluir na lista.
2.  Clique no menu suspenso **Estado da instância**.
3.  Escolha **Terminar instância**.
4.  Na janela de confirmação, clique em **Terminar**.
5.  O estado da instância mudará para `desligando` e, em seguida, `terminada`. Após um tempo, ela desaparecerá da lista.

# Guia de Otimização de Custos do Amazon EC2

A Amazon oferece diferentes modelos de preços e um framework claro para otimizar seus gastos com instâncias EC2.

---

## Parte 1: Conhecendo os Modelos de Preços do EC2

* **Instâncias Sob Demanda (On-Demand):**
    * Têm o menor custo inicial e a maior flexibilidade.
    * Não há compromissos iniciais ou contratos de longo prazo.
    * São elegíveis para o nível gratuito da AWS.

* **Hosts Dedicados (Dedicated Hosts):**
    * São servidores físicos com capacidade dedicada para seu uso.
    * Permitem que você use suas licenças de software existentes (ex: Microsoft SQL Server).

* **Instâncias Dedicadas (Dedicated Instances):**
    * São instâncias que você executa em uma VPC em hardware dedicado a um único cliente.

* **Instâncias Reservadas (Reserved Instances - RIs):**
    * Permitem reservar capacidade por períodos de **1 ou 3 anos**.
    * Oferecem baixos custos de execução por hora, com um preço de uso com desconto que é fixo.

* **Instâncias Spot Reservadas Programadas:**
    * Permitem comprar reservas de capacidade que recorrem em uma base diária, semanal ou mensal, com duração específica, por um termo de 1 ano.

* **Instâncias Spot (Spot Instances):**
    * Permitem que você dê lances em capacidade de instância EC2 não utilizada, o que pode reduzir drasticamente seus custos.
    * O preço por hora flutua com a oferta e a demanda. Sua instância roda enquanto seu lance exceder o preço de mercado.

> **Nota sobre Faturamento:** O **faturamento por segundo** está disponível para instâncias Sob Demanda, Reservadas e Spot que rodam em Amazon Linux ou Ubuntu.

---

## Parte 2: Quando Usar Cada Modelo de Preço (Casos de Uso)

* **Instâncias Sob Demanda:** Ideal para cargas de trabalho com picos (**spiky**), imprevisíveis ou de curto prazo, como ambientes de desenvolvimento e teste.
* **Instâncias Spot:** Ideal para aplicações **tolerantes a falhas** e que podem ser interrompidas (com um aviso de 2 minutos). Casos de uso comuns incluem servidores web, backends de API e processamento de big data.
* **Instâncias Reservadas:** Ideal para cargas de trabalho de **longo prazo** com padrões de uso previsíveis e consistentes.
* **Hosts Dedicados:** Ideal quando você tem **restrições de licenciamento** de software ou precisa atender a requisitos específicos de conformidade e regulamentação.

---

## Parte 3: Os Quatro Pilares da Otimização de Custos

Para otimizar os custos de forma eficaz, você deve considerar os seguintes quatro pilares:

### Pilar 1: Dimensionar Corretamente (Right-sizing)
* **O que é?** Escolher o equilíbrio certo de tipos de instância.
* **Ações:**
    * Use as métricas do **Amazon CloudWatch** (CPU, RAM, rede) para revisar seus recursos e identificar instâncias que podem ser diminuídas (*downsized*).
    * Selecione a instância mais econômica disponível que ainda atenda aos seus requisitos de desempenho.
    * Desligue servidores quando eles não estiverem em uso.
    * Se o padrão de uso for consistente, compre **Instâncias Reservadas**.

### Pilar 2: Aumentar a Elasticidade
* **O que é?** Projetar suas implantações para reduzir a quantidade de capacidade de servidor que fica ociosa.
* **Ações:**
    * **Parar ou hibernar** instâncias com volumes EBS quando não estiverem em uso (especialmente em ambientes de desenvolvimento e teste).
    * Para cargas de produção, configure políticas de **Auto Scaling** precisas e granulares para escalar horizontalmente e atender aos picos de demanda, sem pagar por essa capacidade o tempo todo.

### Pilar 3: Escolher o Modelo de Preço Ideal
* **O que é?** Analisar seus padrões de uso para executar instâncias com a combinação certa de opções de preço.
* **Ações:**
    * **Combine múltiplos tipos de compra** (On-Demand, RIs, Spot) para otimizar os preços com base nas suas necessidades de capacidade atuais e futuras.
    * **Reavalie a arquitetura:** A funcionalidade precisa mesmo rodar em uma EC2, ou poderia ser migrada para uma solução mais barata como o **AWS Lambda**?

### Pilar 4: Otimizar as Escolhas de Armazenamento
* **O que é?** Reduzir custos de armazenamento mantendo a performance e a disponibilidade.
* **Ações:**
    * **Redimensione volumes EBS** que estão superdimensionados.
    * Escolha o **tipo de volume EBS** mais econômico que ainda atenda aos seus requisitos.
    * **Exclua snapshots de EBS** que não são mais necessários.
    * Identifique o destino de armazenamento mais apropriado para os dados (EBS vs. S3).
    * Configure **políticas de ciclo de vida de dados** para migrar dados mais antigos para locais mais baratos, como o **Amazon S3 Glacier**.

---

## Parte 4: A Otimização de Custos como um Processo Contínuo

A otimização de custos não é um processo único. Você deve medir e analisar rotineiramente seu sistema.

### Ferramentas e Boas Práticas
* **Tags de Alocação de Custos:** Ative-as no console de Faturamento e Gerenciamento de Custos para gerar relatórios detalhados e organizar seus custos por categorias de negócio.
* **AWS Trusted Advisor:** Use este serviço para obter orientação em tempo real sobre as melhores práticas da AWS, incluindo otimização de custos.
* **AWS Cost Explorer:** Use esta ferramenta gratuita para visualizar seus custos em gráficos e entender seus gastos.
* **Arquitetar para o Custo:** Incentive as equipes a considerar o custo como um pilar fundamental ao projetar suas arquiteturas.
* **Designar Responsabilidade:** Os esforços de otimização de custos são mais bem-sucedidos quando a responsabilidade é atribuída a um indivíduo ou a uma equipe específica.

# Guia de Serviços de Contêiner na AWS

## Parte 1: Conceitos Fundamentais

### O que são Contêineres?
Contêineres são um método de **virtualização de sistema operacional**. Eles rodam como processos isolados em termos de recursos e compartilham um sistema operacional virtualizado, em vez de conter um sistema operacional inteiro como as máquinas virtuais.

#### Benefícios dos Contêineres
* **Repetibilidade e Consistência:** O código, as configurações e as dependências da aplicação são empacotados em ambientes de execução autocontidos.
* **Implantação Rápida e Confiável:** Ajudam a garantir que as aplicações sejam implantadas de forma consistente, independentemente do ambiente.
* **Leveza e Velocidade:** As imagens de contêiner são muito menores que as de VMs, e um contêiner é iniciado em centenas de milissegundos.

### O Papel do Docker
O Docker é uma plataforma de software que empacota aplicações em contêineres. Ele é instalado em um servidor host e fornece comandos para construir, iniciar e parar contêineres. Os contêineres são criados a partir de modelos chamados **imagens Docker**, que contêm tudo o que a aplicação precisa para rodar (bibliotecas, ferramentas, código, etc.).

### Contêineres vs. Máquinas Virtuais (VMs): A Diferença Crucial
* **Máquinas Virtuais (VMs):** Rodam diretamente em um **hypervisor**. Cada VM tem seu próprio sistema operacional completo e fornece isolamento de processo no nível da VM. (Exemplo: 3 aplicações rodando em 3 instâncias EC2 separadas).
* **Contêineres:** Rodam sobre um sistema operacional convidado (host) que possui um motor de contêiner (como o Docker). Múltiplos contêineres compartilham o kernel do SO host e fornecem isolamento de processo no nível do contêiner. (Exemplo: 3 aplicações em 3 contêineres rodando em uma única instância EC2).

---

## Parte 2: Amazon Elastic Container Service (ECS) - Orquestração Docker Gerenciada

O Amazon ECS é um serviço de gerenciamento de contêineres escalável e de alto desempenho que **orquestra a execução de contêineres Docker**. Ele gerencia a frota de instâncias EC2 (nós) para você, removendo a complexidade de gerenciar a infraestrutura.

### Componentes do ECS
* **Definição de Tarefa (Task Definition):** É o "projeto" ou "blueprint" da sua aplicação, especificando quais contêineres devem ser executados para a tarefa.
* **Agendador de Tarefas (Task Scheduler):** É o componente do ECS responsável por posicionar as tarefas (contêineres) dentro do seu cluster, considerando os recursos de CPU e memória.
* **Cluster ECS:** É o agrupamento lógico de recursos onde suas tarefas são executadas.

### Os Tipos de Inicialização (Launch Types): A Escolha de Gerenciamento

#### 1. Tipo de Inicialização EC2: Controle Total
* **Como funciona?** O cluster ECS consiste em um grupo de **instâncias EC2 que você gerencia**.
* **Quando usar?** Quando você precisa de **controle granular** sobre a infraestrutura subjacente, como escolher tipos de instância específicos, gerenciar patches, etc.

#### 2. Tipo de Inicialização Fargate: Abordagem Serverless
* **Como funciona?** O cluster é **gerenciado pela AWS**. Você não vê ou gerencia as instâncias EC2 subjacentes.
* **Quando usar?** Quando você quer se concentrar apenas em construir e empacotar sua aplicação, sem se preocupar em provisionar, configurar ou escalar o cluster de servidores. É uma abordagem que remove a sobrecarga operacional.

---

## Parte 3: Amazon Elastic Kubernetes Service (EKS) - Kubernetes Gerenciado

### Primeiro, o que é Kubernetes?
Kubernetes (também conhecido como K8s) é um popular **software de código aberto para orquestração de contêineres**. Ele permite implantar e gerenciar aplicações em contêineres em escala, automatizando o provisionamento, a rede, a distribuição de carga e o escalonamento.

### O que é o Amazon EKS?
O Amazon EKS é o serviço gerenciado da AWS que **facilita a execução do Kubernetes na AWS**. Ele remove a necessidade de você instalar, operar e manter seu próprio plano de controle do Kubernetes.
* **Compatibilidade:** O EKS é um Kubernetes certificado, então aplicações que já rodam em Kubernetes são compatíveis. Ele suporta contêineres Linux e Windows.
* **ECS vs. EKS:** A AWS oferece ambos os orquestradores (ECS e EKS) para fornecer aos clientes opções flexíveis, permitindo que escolham a que melhor se adapta às suas necessidades e conhecimento prévio.

---

## Parte 4: Amazon Elastic Container Registry (ECR) - Armazenamento de Imagens

### O Problema que Resolve
O desafio de rastrear, armazenar e gerenciar de forma segura as imagens de contêiner.

### O que é?
O Amazon ECR é um **registro de contêineres Docker totalmente gerenciado** que facilita para os desenvolvedores armazenar, gerenciar e implantar imagens de contêineres Docker.

### Como Funciona e Integrações
* **Integração com ECS:** Você especifica o repositório ECR em sua Definição de Tarefa, e o ECS busca as imagens apropriadas para suas aplicações.
* **Integração com EKS:** Também é possível usar imagens do Amazon ECR com o Amazon EKS.
* **Recursos Adicionais:** Suporta colaboração em equipe, controle de acesso e integração com ferramentas de terceiros.

# Guia Completo do AWS Lambda (Computação Serverless)

## Parte 1: O que é o Lambda e Seus Benefícios?

### A Abordagem Serverless
Enquanto o Amazon EC2 oferece máquinas virtuais (IaaS) e o ECS/EKS oferecem serviços de contêiner, o AWS Lambda representa uma terceira abordagem: a **computação sem servidor (serverless)**.

O Lambda é um serviço sem servidor e **orientado a eventos** que permite que você execute código sem provisionar ou gerenciar servidores. Você cria uma **função Lambda**, que é um recurso da AWS contendo seu código, e a configura para ser acionada (disparada) em resposta a um evento ou em um cronograma.

### Principais Benefícios
* **Sem Gerenciamento de Servidores:** O Lambda automatiza completamente a administração, gerenciando toda a infraestrutura para executar seu código em uma plataforma de alta disponibilidade e tolerante a falhas. Isso permite que você se concentre na construção dos seus serviços.
* **Pagamento por Uso:** Seu código só é executado quando é acionado. Você **paga apenas pelo tempo de computação que consome** e não é cobrado quando seu código não está em execução. O faturamento é medido em incrementos de 100 milissegundos.
* **Facilidade de Uso:** Não há novas linguagens, ferramentas ou frameworks para aprender. O Lambda suporta várias linguagens de programação, incluindo Java, Go, PowerShell, Node.js, C#, Python e Ruby.
* **Tolerância a Falhas Integrada:** O Lambda mantém capacidade de computação em várias Zonas de Disponibilidade em cada região para proteger o código contra falhas de máquinas ou data centers.
* **Orquestração:** Para tarefas complexas ou de longa duração, você pode orquestrar múltiplas funções Lambda construindo fluxos de trabalho com o **AWS Step Functions**.

---

## Parte 2: Como as Funções são Acionadas (Fontes de Eventos / Triggers)
As funções Lambda são acionadas por **fontes de eventos**. Existem diferentes modelos de invocação:

* **Modelo "Push" (Invocação Direta por Serviços AWS):** Alguns serviços publicam eventos que invocam a função Lambda diretamente.
    * **Exemplos:** Amazon S3, Amazon CloudWatch Events.
* **Modelo "Pull" (Sondagem pelo Lambda):** O Lambda busca (faz "pull") registros de outros serviços.
    * **Exemplos:** Amazon Simple Queue Service (SQS), Amazon DynamoDB.
* **Invocação Síncrona/Direta:** Outros serviços podem invocar sua função Lambda diretamente e aguardar uma resposta. Você também pode invocar a função diretamente.
    * **Exemplos:** Elastic Load Balancing, Amazon API Gateway, Console do Lambda, API, SDK ou AWS CLI.
* **Monitoramento:** O Lambda monitora automaticamente as funções e registra todas as solicitações no **Amazon CloudWatch** para ajudar na solução de problemas.

---

## Parte 3: Guia de Configuração de uma Função Lambda
Ao criar uma função Lambda no Console de Gerenciamento da AWS, você precisa configurar os seguintes itens:

### Passos Essenciais
1.  **Dar um Nome** à função.
2.  **Especificar o Ambiente de Execução (Runtime):** A linguagem que a função usará (ex: Python, Node.js).
3.  **Definir uma Função de Execução (Execution Role):** Uma função do IAM que concede as permissões necessárias para a função interagir com outros serviços da AWS.

### Configurações da Função
* **Adicionar um Gatilho (Trigger):** A fonte de evento que acionará a função.
* **Adicionar o Código da Função:** Você pode usar o editor de código no console ou fazer o upload de um arquivo.
* **Definir a Memória:** A quantidade de memória em megabytes a ser alocada para a função (até 3008 MB).
* **(Opcional) Configurações Avançadas:** Variáveis de ambiente, tempo limite (timeout), a VPC onde a função será executada, e outras.

### O Pacote de Implantação (Deployment Package)
Todas as configurações, código e dependências são colocados em um pacote de implantação, que é um arquivo ZIP. Ao usar o console do Lambda, ele gerencia esse pacote para você. Se usar a API, você precisa criá-lo.

---

## Parte 4: Casos de Uso Práticos

### Caso de Uso 1: Baseado em Cronograma (Agendamento)
* **Objetivo:** Parar instâncias EC2 à noite e iniciá-las pela manhã para economizar custos.
* **Como Funciona:**
    1.  Um **Amazon CloudWatch Event** é agendado para ser executado em horários específicos.
    2.  O evento **aciona uma função Lambda**.
    3.  A função Lambda, usando sua Role do IAM com permissões, **executa a ação de parar ou iniciar** as instâncias EC2.

### Caso de Uso 2: Orientado a Eventos
* **Objetivo:** Criar miniaturas (thumbnails) de cada imagem que é carregada em um bucket S3.
* **Como Funciona:**
    1.  Um **upload de objeto no bucket S3 de origem** é o evento.
    2.  Este evento **aciona a função Lambda**.
    3.  A função Lambda lê o objeto de imagem, cria uma miniatura e a salva em um **bucket S3 de destino**.

---

## Parte 5: Limites Importantes do Serviço
Existem alguns limites de recursos a serem conhecidos:

* **Memória:** A alocação máxima de memória para uma única função é de **3008 MB**.
* **Execuções Simultâneas:** O limite é de **1.000** execuções simultâneas por região.
* **Tempo de Execução (Timeout):** As funções podem ser configuradas para rodar por até **15 minutos**. Você pode definir qualquer valor entre 1 segundo e 15 minutos.
* **Tamanho do Pacote de Implantação:** O limite é de **250 MB**.
* **Camadas (Layers):** São arquivos ZIP que contêm bibliotecas ou outras dependências. Com as camadas, você pode usar bibliotecas sem precisar incluí-las diretamente no seu pacote de implantação.
* **Tipos de Limites:** Limites podem ser **flexíveis (soft)**, que podem ser aumentados via ticket de suporte, ou **rígidos (hard)**, que não podem ser aumentados.

# Guia do AWS Elastic Beanstalk (Plataforma como Serviço - PaaS)

## O que é o Elastic Beanstalk?
O Elastic Beanstalk é um serviço de computação da AWS que fornece uma maneira fácil de colocar **aplicações web** em funcionamento na nuvem AWS. A premissa central é:

> **Você faz o upload do seu código, e o Elastic Beanstalk lida automaticamente com a implantação.**

---

## O que o Elastic Beanstalk Gerencia Automaticamente?
Ele cuida de toda a complexidade da infraestrutura para que você possa focar no seu código. As tarefas automatizadas incluem:
* Provisionamento e configuração da infraestrutura.
* Implantação (Deployment).
* Balanceamento de Carga (Load Balancing).
* Escalonamento Automático (Auto Scaling).
* Monitoramento de Saúde (Health Monitoring).
* Análise e Depuração.
* Registro de Logs.

---

## Modelo de Preços e Plataformas Suportadas

### Modelo de Preços
* **Não há custo adicional pelo serviço Elastic Beanstalk em si.**
* Você paga apenas pelos recursos da AWS que ele cria para executar sua aplicação (ex: instâncias EC2, buckets S3). O modelo é "pague apenas pelo que usar".

### Como Implantar o Código?
Você pode implantar sua aplicação através de várias ferramentas:
* Console de Gerenciamento da AWS
* Interface de Linha de Comando da AWS (CLI)
* Repositório Git
* IDEs como Eclipse ou Visual Studio

### Plataformas Suportadas
Ele suporta uma ampla gama de plataformas e tecnologias:
* Java
* .NET
* PHP
* Node.js
* Python
* Ruby
* Go
* Docker

---

## Principais Vantagens e Benefícios

### 1. Rápido e Simples de Usar
É uma das maneiras mais rápidas de começar a rodar uma aplicação na AWS. Você sobe sua aplicação e o serviço cuida do resto.

### 2. Aumenta a Produtividade do Desenvolvedor
Você pode focar em escrever código em vez de se preocupar em gerenciar e configurar:
* Servidores
* Bancos de dados
* Balanceadores de carga
* Firewalls
* Redes

### 3. Escalabilidade Automática ("Acompanha o seu Crescimento")
Sua aplicação pode lidar com picos de carga de trabalho ou tráfego. O Elastic Beanstalk escala sua aplicação automaticamente para cima e para baixo com base nas necessidades específicas, usando configurações de escalonamento automático facilmente ajustáveis (que podem ser baseadas em métricas como a utilização de CPU).

### 4. Controle Total (se necessário)
Apesar da automação, você não perde o controle.
* **Liberdade de Escolha:** Você pode selecionar os recursos da AWS que são ideais para sua aplicação, como o tipo de instância Amazon EC2.
* **Acesso aos Recursos:** Você mantém controle total sobre os recursos subjacentes que alimentam sua aplicação e pode acessá-los a qualquer momento.
* **Gerenciamento Flexível:** Se você decidir que quer assumir o controle de alguns ou de todos os elementos da sua infraestrutura, pode fazê-lo usando as capacidades de gerenciamento do Elastic Beanstalk.

# Módulo 6: Revisão Final e Questão Prática

## Checklist de Aprendizagem do Módulo

Neste módulo, você aprendeu a:

* Fornecer uma visão geral dos diferentes serviços de computação da AWS na nuvem.
* Demonstrar quando usar o Amazon Elastic Compute Cloud (Amazon EC2).
* Identificar a funcionalidade no console do Amazon EC2.
* Realizar funções básicas no Amazon EC2 para construir um ambiente de computação virtual.
* Identificar os elementos de otimização de custos do Amazon EC2.
* Demonstrar quando usar o AWS Elastic Beanstalk.
* Demonstrar quando usar o AWS Lambda.
* Identificar como executar aplicações em contêineres em um cluster de servidores gerenciados.

---

## Análise de Questão Prática (Exemplo de Exame)

### A Pergunta

> "Qual serviço da AWS ajuda os desenvolvedores a implantar rapidamente recursos que podem fazer uso de diferentes linguagens de programação, como .NET e Java?"

### Análise das Palavras-Chave

* **"Desenvolvedores implantam recursos rapidamente":** Indica que o foco da questão é fornecer aos desenvolvedores uma maneira de implantar aplicações rapidamente.
* **"Diferentes linguagens de programação":** É a frase-chave que descreve o caso de uso de como os desenvolvedores querem usar os recursos da AWS.

### A Resposta Correta e a Justificativa

Ao identificar os componentes-chave que os desenvolvedores precisavam, podemos determinar que a resposta correta é **C, AWS Elastic Beanstalk**.

A capacidade dos desenvolvedores de implantar rapidamente a infraestrutura da AWS para suas aplicações **aumenta a produtividade do desenvolvedor**, pois eles só precisam se concentrar em escrever o código para a aplicação e não em provisionar ou gerenciar a infraestrutura subjacente.
