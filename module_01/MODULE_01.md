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
