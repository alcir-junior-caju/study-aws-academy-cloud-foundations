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
