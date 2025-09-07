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
