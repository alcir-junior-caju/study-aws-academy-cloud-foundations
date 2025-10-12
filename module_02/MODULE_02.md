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
