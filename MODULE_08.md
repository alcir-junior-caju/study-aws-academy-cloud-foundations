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

# Módulo 8: Bancos de Dados

## A Importância dos Bancos de Dados
O mundo dos negócios está em constante mudança e evolução. Ao registrar, atualizar e rastrear dados com precisão, de forma eficiente e regular, as empresas podem usar o imenso potencial dos insights que obtêm de seus dados. Os sistemas de gerenciamento de banco de dados são o elo crucial para gerenciar esses dados. Assim como outros serviços em nuvem, os bancos de dados em nuvem oferecem vantagens de custo significativas em relação aos bancos de dados tradicionais.

---

## O que Vamos Aprender?

### Serviços Abordados
* **Amazon Relational Database Service (Amazon RDS)**
* **Amazon DynamoDB**
* **Amazon Redshift**
* **Amazon Aurora**

### Principais Conceitos
* As diferenças entre soluções de banco de dados **gerenciadas e não gerenciadas**.
* As diferenças entre um banco de dados **SQL e um NoSQL**.
* Como combinar um serviço de banco de dados a um conjunto específico de requisitos de negócios.

---

## Recursos de Aprendizagem Disponíveis
* **Demonstrações gravadas:** Mostrando como interagir com o RDS e o DynamoDB.
* **Laboratório prático (Hands-on):** Para praticar a criação de um banco de dados com o Amazon RDS.
* **Verificação de conhecimento:** Para testar sua compreensão dos conceitos-chave.

---

## Objetivos de Aprendizagem
Ao final deste módulo, você será capaz de:
* Explicar a funcionalidade do Amazon RDS, Amazon DynamoDB, Amazon Redshift e Amazon Aurora.
* Realizar tarefas básicas em um banco de dados RDS (lançar, configurar e consultar).
* Descrever as diferenças entre um banco de dados SQL e um NoSQL.
* Combinar o serviço de banco de dados apropriado a um conjunto de requisitos de dados.

# Guia do Amazon RDS: Bancos de Dados Relacionais Gerenciados

## Parte 1: Gerenciado vs. Não Gerenciado - A Diferença Chave

As soluções de banco de dados na nuvem geralmente se enquadram em uma de duas categorias.

### Serviços Não Gerenciados
* **O que são?** Serviços provisionados em porções discretas, onde **você** gerencia como o serviço responde a mudanças na carga, erros e disponibilidade.
* **Exemplo:** Instalar um sistema de gerenciamento de banco de dados relacional (como MySQL) em uma **instância Amazon EC2**. Isso é muito semelhante a executar um banco de dados em seu próprio data center.
* **Benefício:** Você tem um controle mais refinado sobre a configuração e o comportamento do seu banco de dados.

### Serviços Gerenciados
* **O que são?** Serviços que, embora permitam configuração, exigem muito menos gerenciamento da sua parte, pois a AWS cuida da infraestrutura e das tarefas administrativas.
* **Exemplo:** Amazon RDS.

### Os Desafios de um Banco de Dados Não Gerenciado
Quando você executa seu próprio banco de dados, você é responsável por várias tarefas administrativas que consomem tempo e exigem especialização:
* Manutenção de servidores e consumo de energia.
* Instalação e aplicação de patches de software (updates).
* Backups de banco de dados.
* Garantir a alta disponibilidade.
* Planejar a escalabilidade.
* Segurança dos dados.
* Instalação e aplicação de patches do sistema operacional.

---

## Parte 2: Amazon RDS - O que é e o que ele faz por você

### Definição
O Amazon RDS é um serviço gerenciado que **configura, opera e escala bancos de dados relacionais** sem qualquer administração contínua da sua parte.

### Seu Foco vs. Foco do RDS
* **Seu Foco:** Seus dados e a otimização da sua aplicação.
* **Foco do RDS (O que ele gerencia para você):**
    * Instalação e patches do sistema operacional e do software do banco de dados.
    * Backups automáticos.
    * Alta disponibilidade.
    * Escalabilidade.
    * Gerenciamento de energia e servidores.
    * Manutenção.

Transferir essas operações para o RDS reduz sua carga de trabalho operacional e os custos associados.

---

## Parte 3: Detalhes e Funcionalidades Essenciais do RDS

* **Componente Básico:** A **instância de banco de dados**, que é um ambiente de banco de dados isolado.
* **Configuração:** Ao criar, você escolhe uma **classe de instância** (hardware) e o **tipo de armazenamento**, equilibrando performance e custo.
* **Mecanismos de Banco de Dados (Engines) Suportados:**
    * MySQL
    * Amazon Aurora
    * Microsoft SQL Server
    * PostgreSQL
    * MariaDB
    * Oracle
* **Rede (Networking):** Pode ser executado em uma VPC, onde você controla o ambiente de rede (IPs, sub-redes, ACLs). A boa prática é isolar a instância de banco de dados em uma **sub-rede privada**.

### Funcionalidade 1: Implantação Multi-AZ (Alta Disponibilidade)
* **O que é?** Uma das características mais poderosas do RDS para garantir alta disponibilidade.
* **Como funciona?** O RDS cria automaticamente uma **cópia de standby (reserva)** da sua instância de banco de dados em **outra Zona de Disponibilidade**. As transações são **replicadas de forma síncrona**.
* **Failover:** Se a instância principal falhar, o RDS promove automaticamente a instância de standby para se tornar a nova principal. Sua aplicação não precisa ser alterada, pois ela se conecta a um endpoint de DNS que o RDS atualiza.

### Funcionalidade 2: Réplicas de Leitura (Read Replicas) - Performance
* **O que é?** Uma forma de reduzir a carga na sua instância de banco de dados principal, especialmente para aplicações com alto volume de leituras.
* **Como funciona?** As atualizações da instância de origem são **copiadas de forma assíncrona** para uma ou mais instâncias de réplica de leitura. Você direciona as consultas de leitura (`SELECT`) para as réplicas.
* **Motores Suportados:** MySQL, MariaDB, PostgreSQL e Amazon Aurora.

---

## Parte 4: Quando Usar (e não usar) o RDS?

### Cenários Ideais para o RDS
Aplicações web e móveis que precisam de um banco de dados com alta taxa de transferência, escalabilidade massiva de armazenamento e alta disponibilidade. O RDS é uma boa solução se você:
* Precisa suportar transações ou consultas complexas.
* Tem uma taxa de consulta ou escrita de média a alta (até 30.000 IOPS).
* Não precisa de mais de um único nó de trabalho ou "shard".

### Cenários onde o RDS PODE NÃO ser a Melhor Solução
Considere outras opções se você:
* Precisa de leituras/escritas massivas (ex: 150.000 escritas por segundo).
* Tem conjuntos de dados muito grandes ou demandas de taxa de transferência extremas.
* Tem apenas requisições simples de `get` ou `put` e consultas que poderiam ser mais adequadas para um banco de dados NoSQL (como o Amazon DynamoDB).

---

## Parte 5: Entendendo os Custos do RDS
* **Horas de Serviço:** Você é cobrado pelo tempo em que sua instância de banco de dados está em execução.
* **Características da Instância:** O mecanismo, o tamanho da instância e a classe de memória afetam o custo.
* **Tipo de Compra:**
    * **Instâncias Sob Demanda (On-Demand):** Pague por hora, sem compromissos.
    * **Instâncias Reservadas (Reserved Instances):** Faça um pagamento inicial único para reservar uma instância por 1 ou 3 anos, com um custo por hora menor.
* **Número de Instâncias:** Provisionar múltiplas instâncias (ex: para réplicas de leitura) impacta o custo.
* **Armazenamento de Backup:** O armazenamento de backup é **gratuito até 100%** do seu armazenamento de banco de dados provisionado. Após a instância ser terminada, o backup é cobrado por GB/mês.
* **Requisições de I/O e Transferência de Dados:** Você é cobrado pelo número de requisições de I/O. A transferência de dados **de entrada é gratuita**, e a de **saída** tem custos escalonados (tiered).

# Como Criar e Conectar a um Banco de Dados MySQL no Amazon RDS (Guia Prático)

Este guia mostra o passo a passo para criar um banco de dados MySQL gerenciado com o RDS e conectar a ele a partir de uma instância EC2.

---

## Parte 1: Criação do Banco de Dados no Console da AWS

### Passo 1: Iniciar o Assistente de Criação
1.  No Console da AWS, navegue até o serviço **RDS**.
2.  No painel principal, clique no botão **Criar banco de dados (Create database)**.

### Passo 2: Escolher o Mecanismo (Engine) e o Caso de Uso
1.  Em "Escolha um método de criação", mantenha **Criação padrão**.
2.  Em "Opções de mecanismo", selecione **MySQL**.
3.  Na seção "Templates", escolha **Nível gratuito (Free tier)** para este guia, o que simplifica as opções e evita custos.

### Passo 3: Definir as Especificações da Instância
1.  **Identificador da Instância de BD:** Dê um nome único ao seu banco de dados (ex: `myacfdb`).
2.  **Credenciais:**
    * **Nome de usuário mestre:** Defina o usuário administrador (ex: `admin`).
    * **Senha mestra:** Crie e confirme uma senha segura.
3.  **Classe da Instância de BD:** O nível gratuito selecionará automaticamente uma classe como `db.t2.micro`.
4.  **Armazenamento:** Deixe as configurações padrão e desabilite o "storage autoscaling" (dimensionamento automático de armazenamento).
5.  **Disponibilidade e Durabilidade:** Para o nível gratuito, a opção de implantação Multi-AZ não estará disponível.

### Passo 4: Configurar a Conectividade
1.  **VPC:** Selecione a Virtual Private Cloud onde sua instância EC2 (que vai se conectar ao banco) está localizada (ex: `lab VPC`).
2.  **Acessibilidade Pública:** Defina como **Não**. Esta é a prática de segurança recomendada, tornando o banco de dados acessível apenas de dentro da sua VPC.
3.  **Grupo de Segurança da VPC (Firewall):**
    * Escolha **Selecionar existente**.
    * Selecione um grupo de segurança que permita tráfego na porta do MySQL (`3306`) a partir da sua instância EC2 ou do grupo de segurança dela.
4.  **Zona de Disponibilidade:** Pode deixar como "Sem preferência".
5.  **Porta do Banco de Dados:** Mantenha a padrão (`3306`).

### Passo 5: Configurações Adicionais
1.  **Autenticação de Banco de Dados:** Mantenha **Autenticação por senha**.
2.  Expanda a seção **Configurações adicionais**. Para um ambiente de desenvolvimento e para simplificar, você pode desabilitar várias opções:
    * **Backup:** Altere o período de retenção para **0 dias** para desabilitar backups automáticos.
    * **Criptografia:** Deixe desmarcada.
    * **Monitoramento Aprimorado:** Deixe desmarcado.
    * **Atualizações automáticas de versões secundárias:** Desmarque.
    * **Proteção contra exclusão:** Desmarque esta opção para que você possa excluir o banco de dados facilmente ao final dos testes.

### Passo 6: Criar e Monitorar
1.  Revise o painel de **Custo mensal estimado**.
2.  Clique em **Criar banco de dados**.
3.  Você será levado à lista de bancos de dados. Aguarde o **Status** da sua nova instância mudar de `Criando` para `Disponível`. Isso pode levar alguns minutos.
4.  **AÇÃO IMPORTANTE:** Após a criação, clique no nome da sua instância de BD. Na aba **Conectividade e segurança**, encontre o valor do **Endpoint** e copie-o para um editor de texto. Você precisará dele para se conectar.

---

## Parte 2: Conexão e Teste a partir de uma Instância EC2

### Passo 7: Conectar ao Banco de Dados
1.  Conecte-se via SSH à sua instância EC2 que está na mesma VPC do seu RDS.
2.  No terminal da instância, use o cliente de linha de comando do MySQL para se conectar. Substitua `[COLE_O_ENDPOINT_AQUI]` pelo valor que você copiou:
    ```bash
    mysql -h [COLE_O_ENDPOINT_AQUI] -u admin -p
    ```
3.  Quando solicitado (`Enter password:`), digite a senha mestra que você definiu durante a criação.

### Passo 8: Criar Tabela, Inserir e Consultar Dados
1.  Uma vez conectado, você verá o prompt do MySQL (`mysql>`). Agora você pode executar comandos SQL padrão.
2.  **Crie uma tabela:**
    ```sql
    CREATE TABLE MyContacts (FirstName VARCHAR(20), LastName VARCHAR(20), Phone VARCHAR(20));
    ```
3.  **Insira alguns dados:**
    ```sql
    INSERT INTO MyContacts VALUES ('Chris', 'Jones', '555-555-1111');
    INSERT INTO MyContacts VALUES ('Mary', 'Smith', '555-555-2222');
    ```
4.  **Consulte os dados para verificar:**
    ```sql
    SELECT * FROM MyContacts WHERE FirstName='Chris';
    ```
5.  Você deverá ver o registro de "Chris" retornado, confirmando que seu banco de dados está funcionando corretamente.

# Guia do Amazon DynamoDB e a Diferença entre SQL vs. NoSQL

## Parte 1: Bancos de Dados Relacionais (SQL) vs. Não Relacionais (NoSQL)

A primeira etapa para entender o DynamoDB é saber a diferença fundamental entre os dois principais tipos de bancos de dados.

| Bancos de Dados Relacionais (SQL) | Bancos de Dados Não Relacionais (NoSQL) |
| :--- | :--- |
| Trabalha com **dados estruturados**. | Lida com dados **semiestruturados e não estruturados**. |
| Organizado por **tabelas, registros (linhas) e colunas**. | Trabalha com coleções de **documentos** ou listas de **pares de chave-valor**. |
| Pense em uma **planilha**. | Pense em um **documento JSON**. |
| Cria **relacionamentos** entre tabelas. | O modelo não é relacional. |
| Usa **SQL (Structured Query Language)**. | Conhecido como **NoSQL**. |
| Escala **verticalmente** (aumentando a potência de um único servidor). | Escala **horizontalmente** (distribuindo a carga entre muitos servidores), o que os torna ideais para conjuntos de dados massivos. |

---

## Parte 2: Um Mergulho Profundo no Amazon DynamoDB

O DynamoDB é o principal serviço de banco de dados NoSQL da AWS.

### O que é o DynamoDB?
É um serviço de banco de dados NoSQL **rápido e flexível**, projetado para todas as aplicações que precisam de **latências consistentes de milissegundos de um dígito, em qualquer escala**.

### Principais Vantagens e Características
* **Totalmente Gerenciado:** A AWS gerencia toda a estrutura de dados subjacente, o particionamento automático e o armazenamento redundante em uma arquitetura tolerante a falhas.
* **Escalabilidade Ilimitada:** Não há limite prático para o número de itens que você pode armazenar em uma tabela.
* **Esquema Flexível:** Itens na mesma tabela podem ter atributos diferentes. Isso permite que você adicione novos atributos à medida que sua aplicação evolui, sem precisar realizar migrações de esquema complexas.
* **Alta Performance:** Todos os dados no DynamoDB são armazenados em **unidades de estado sólido (SSDs)**, e sua linguagem de consulta simples permite um desempenho consistente e de baixa latência.
* **Taxa de Transferência Provisionada (Throughput):** Você pode provisionar (definir) a quantidade de capacidade de leitura e escrita que sua tabela precisa.
* **Auto Scaling:** Você pode habilitar o dimensionamento automático para que o DynamoDB monitore a carga e aumente ou diminua a taxa de transferência provisionada conforme necessário.
* **Outras Funcionalidades:**
    * **Tabelas Globais:** Permitem replicar automaticamente os dados da sua tabela entre diferentes Regiões da AWS.
    * **Criptografia em Repouso.**
    * **Tempo de Vida (TTL):** Permite definir um tempo de expiração para itens específicos, que serão excluídos automaticamente.

### Os Componentes Fundamentais do DynamoDB
* **Tabelas:** Uma coleção de dados (semelhante a uma tabela SQL).
* **Itens:** Um grupo de atributos que é unicamente identificável (semelhante a uma linha em uma tabela SQL).
* **Atributos:** Um elemento de dado fundamental (semelhante a uma coluna em uma tabela SQL).

### A Estrutura de Chaves Primárias (O Mais Importante!)
Ao criar uma tabela, você **deve** especificar sua chave primária. Ela é usada para identificar unicamente cada item.

#### 1. Chave Primária Simples
* **Composição:** Apenas **um** atributo.
* **Nome do Atributo:** **Chave de Partição (Partition Key)**.
* **Função:** O DynamoDB usa o valor da chave de partição para determinar a partição física onde o item será armazenado. Cada item deve ter um valor de chave de partição único.

#### 2. Chave Primária Composta
* **Composição:** **Dois** atributos.
* **Nomes dos Atributos:**
    1.  **Chave de Partição (Partition Key):** O primeiro atributo.
    2.  **Chave de Classificação (Sort Key):** O segundo atributo.
* **Função:** Múltiplos itens podem ter a mesma chave de partição, mas devem ter valores de chave de classificação diferentes. Os itens com a mesma chave de partição são armazenados juntos, ordenados pela chave de classificação.

# Como Criar e Popular uma Tabela no DynamoDB (Guia Prático)

Este guia mostra o passo a passo para criar uma tabela simples no DynamoDB e populá-la com dados de um arquivo JSON usando a AWS CLI.

## Preparação
* **O Cenário:** O objetivo é criar uma tabela para um catálogo de produtos.
* **Os Dados:** Os dados estão em um arquivo JSON. Cada produto é um item com vários atributos, mas todos têm um atributo `Id` (do tipo número) que é único e servirá como chave.

---

## Parte 1: Criação da Tabela no Console da AWS

### Passo 1: Navegar e Iniciar
1.  No Console da AWS, navegue até o serviço **DynamoDB**.
2.  No painel principal, clique no botão **Criar tabela (Create table)**.

### Passo 2: Configurar a Tabela
1.  **Nome da tabela:** Dê um nome para sua tabela (ex: `product catalog`).
2.  **Chave de partição:** Digite o nome do atributo que será a chave principal (ex: `Id`).
3.  **Tipo de dado:** Selecione o tipo de dado da chave de partição (para este exemplo, `Number` (Número)).
4.  Deixe as outras configurações como padrão.

### Passo 3: Criar
1.  Clique em **Criar tabela**. A criação é quase instantânea.
2.  Após a criação, navegue até a aba **Itens** da sua nova tabela para confirmar que ela está vazia.

---

## Parte 2: Populando a Tabela com a AWS CLI

### Passo 1: Listar as Tabelas (Verificação)
1.  Abra um terminal com a AWS CLI configurada (como o PowerShell para AWS).
2.  Execute o comando `list-tables` para confirmar que sua tabela foi criada e é visível para a CLI.
    ```bash
    aws dynamodb list-tables --region [sua-regiao]
    ```
3.  **Resultado Esperado:** O nome da sua tabela (`product catalog`) deve aparecer na lista de retorno.

### Passo 2: Descrever a Tabela (Verificação Opcional)
1.  Execute o comando `describe-table` para ver os detalhes da sua tabela.
    ```bash
    aws dynamodb describe-table --table-name product-catalog --region [sua-regiao]
    ```
2.  **Resultado Esperado:** O retorno mostrará detalhes como o status da tabela, o tamanho (atualmente 0) e a definição da chave primária (`Id`, do tipo `N` para número).

### Passo 3: Escrever os Itens em Lote (Popular a Tabela)
1.  Use o comando `batch-write-item` para carregar todos os itens do seu arquivo JSON de uma só vez.
    ```bash
    aws dynamodb batch-write-item --request-items file://caminho/para/seu/arquivo.json --region [sua-regiao]
    ```
    *Substitua `caminho/para/seu/arquivo.json` pelo caminho real do seu arquivo de dados.*

---

## Parte 3: Verificação Final no Console

### Passo 1: Atualizar a Visualização
1.  Volte para o console do DynamoDB, na aba **Itens** da sua tabela.
2.  **Atualize a página**.
3.  **Resultado Esperado:** Todos os produtos do seu arquivo JSON devem agora estar listados como itens na tabela.

### Passo 2: Realizar uma Consulta (Scan/Query)
1.  Use a ferramenta de exploração de itens do console para buscar um item específico.
2.  **Exemplo:** Crie um filtro (Scan) onde o atributo `Id` seja igual a `204`.
3.  **Resultado Esperado:** O item correspondente a esse ID será retornado, confirmando que os dados foram carregados e podem ser consultados.

# Guias Finais do Módulo 8: Redshift, Aurora e Revisão

## Guia do Amazon Redshift (Data Warehouse)

### O que é?
O Amazon Redshift é um **data warehouse** rápido e totalmente gerenciado que torna simples e econômico analisar todos os seus dados usando SQL padrão e suas ferramentas de business intelligence (BI) existentes.

### O Problema que Resolve
Construir um data warehouse tradicional é complexo, caro e pode levar meses. O Redshift é uma solução simples, econômica e escalável para executar consultas analíticas complexas em petabytes de dados estruturados.

### Principais Características e Arquitetura

#### Como Funciona a Arquitetura
Uma implementação do Redshift consiste em um cluster com dois tipos de nós:
* **Nó Líder (Leader Node):** Gerencia a comunicação com os clientes, analisa as consultas, desenvolve planos de execução, compila o código e o distribui para os nós de computação. No final, agrega os resultados intermediários.
* **Nós de Computação (Compute Nodes):** Executam o código compilado em paralelo e enviam os resultados parciais de volta ao nó líder.

#### Principais Vantagens
* **Alta Performance:** Utiliza otimização de consulta sofisticada, **armazenamento colunar** e **execução de consultas massivamente paralela**. A maioria dos resultados retorna em segundos.
* **Modelo de Pagamento:** Você paga apenas pelo que usa.
* **Gerenciamento Automatizado:** Automatiza a maioria das tarefas administrativas comuns para gerenciar, monitorar e escalar o cluster, permitindo que você foque nos seus dados.
* **Escalabilidade:** O cluster pode ser escalado para mais ou para menos com alguns cliques no console.
* **Segurança Integrada:** Projetado para fornecer forte criptografia de dados, tanto em repouso quanto em trânsito.
* **Compatibilidade:** Suporta SQL padrão e se conecta com suas ferramentas de BI e clientes SQL existentes através de conectores JDBC e ODBC.

### Casos de Uso Comuns
* **Aumentar a Agilidade:** Migrar data warehouses empresariais tradicionais para o Redshift para poder experimentar com dados em qualquer escala, sem processos de TI complicados.
* **Big Data:** Lidar com quantidades massivas de dados que sobrecarregam sistemas existentes.
* **Self-service BI:** Permite que usuários foquem em consultar e analisar dados, pois o Redshift cuida de muitas das tarefas de implantação e manutenção que exigiriam um DBA.
* **Analytics para SaaS:** Clientes de Software como Serviço podem usar o Redshift para fornecer capacidades analíticas em suas aplicações, implantando um cluster por cliente e usando tags para gerenciar SLAs e faturamento.

---

## Guia do Amazon Aurora (Banco de Dados Relacional Otimizado para Nuvem)

### O que é?
O Amazon Aurora é um banco de dados relacional **compatível com MySQL e PostgreSQL**, mas que foi **construído do zero para a nuvem**.

### Proposta de Valor
Ele combina o **desempenho e a disponibilidade de bancos de dados comerciais de ponta** com a **simplicidade e a economia de bancos de dados de código aberto**.

### Principais Vantagens e Características
* **Totalmente Gerenciado:** Automatiza tarefas demoradas como provisionamento, aplicação de patches, backup, recuperação, detecção de falhas e reparo.
* **Alta Disponibilidade por Design:** A alta disponibilidade é incorporada por padrão na arquitetura, sem necessidade de configuração adicional.
* **Armazenamento Otimizado:** Construído sobre um subsistema de armazenamento distribuído rápido, ideal para grandes conjuntos de dados relacionais.
* **Compatibilidade (Drop-in):** Projetado para ter compatibilidade imediata com os mecanismos MySQL e PostgreSQL, permitindo o uso da maioria das suas ferramentas existentes com pouca ou nenhuma alteração.
* **Modelo de Pagamento:** É um serviço "pague-pelo-uso".
* **Facilidade de Migração:** Funciona perfeitamente com o **AWS Database Migration Service (DMS)** e o **AWS Schema Conversion Tool (SCT)** para simplificar a migração de bancos de dados legados.

### Por que Escolher o Aurora? (Diferenciais)
* **Alta Disponibilidade e Resiliência:** Armazena múltiplas cópias de seus dados em diferentes Zonas de Disponibilidade e faz backup contínuo para o Amazon S3.
* **Performance de Leitura:** Suporta até **15 Réplicas de Leitura (Read Replicas)** para melhorar o desempenho de casos de uso com alto volume de leituras.
* **Recuperação Instantânea de Falhas:** É projetado para reiniciar em **menos de 60 segundos** após uma falha. Ao contrário dos bancos tradicionais, ele não precisa reproduzir o "redo log" do último checkpoint.
* **Cache de Buffer Otimizado:** A arquitetura do Aurora remove o cache de buffer do processo do banco de dados. Isso significa que, após um reinício, o cache está disponível imediatamente, evitando a necessidade de "aquecer" o cache e limitar o acesso.

---

## Módulo de Bancos de Dados: Revisão Final e Questão Prática

### Checklist de Aprendizagem do Módulo
Em resumo, neste módulo você aprendeu a:
* Descrever a diferença entre um banco de dados SQL e NoSQL.
* Explicar e descrever a funcionalidade do Amazon RDS, Amazon DynamoDB, Amazon Redshift e Amazon Aurora.
* Realizar tarefas em um banco de dados RDS, como lançar, configurar e interagir.
* Reconhecer casos de uso comuns para cada um dos quatro serviços de banco de dados cobertos.

### Análise de Questão Prática
* **A Pergunta:** "Qual dos seguintes é um serviço de banco de dados NoSQL totalmente gerenciado?"
* **A Palavra-Chave:** "NoSQL".
* **A Resposta Correta e a Justificativa:** A resposta correta é **B, Amazon DynamoDB**. Embora Aurora, Redshift e DynamoDB sejam todos serviços gerenciados, o DynamoDB é o único que é um serviço de banco de dados NoSQL.
