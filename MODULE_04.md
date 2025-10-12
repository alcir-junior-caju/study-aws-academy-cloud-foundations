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
