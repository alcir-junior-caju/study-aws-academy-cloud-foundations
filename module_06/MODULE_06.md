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
