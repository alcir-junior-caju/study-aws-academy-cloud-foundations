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
