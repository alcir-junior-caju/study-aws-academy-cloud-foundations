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

# Módulo 7: Serviços de Armazenamento da AWS

## Por que o Armazenamento em Nuvem?
O armazenamento em nuvem é um componente crítico da computação em nuvem, pois guarda as informações que as aplicações usam. Análise de big data, data warehouses, a Internet das Coisas (IoT), bancos de dados e aplicações de backup e arquivamento, todos dependem de alguma forma de arquitetura de armazenamento de dados.

O armazenamento em nuvem é tipicamente:
* Mais confiável
* Mais escalável
* Mais seguro
... do que os sistemas de armazenamento locais (on-premises) tradicionais.

---

## Serviços Abordados no Módulo
Neste módulo, revisaremos os seguintes serviços de armazenamento da AWS:
* **Amazon Elastic Block Store (Amazon EBS)**
* **Amazon Simple Storage Service (Amazon S3)**
* **Amazon Elastic File System (Amazon EFS)**
* **Amazon S3 Glacier**

---

## Objetivos de Aprendizagem
O objetivo deste módulo é aprender a descrever os conceitos-chave para o Armazenamento da AWS. Você aprenderá sobre os diferentes tipos de recursos de armazenamento e revisará as opções de preço que afetam o custo do armazenamento.

Ao final deste módulo, você será capaz de:
* Identificar os diferentes tipos de armazenamento.
* Explicar e descrever a funcionalidade do Amazon Simple Storage Service (S3), Amazon Elastic Block Store (EBS), Amazon Elastic File System (EFS) e Amazon S3 Glacier.

# Guia Completo do Amazon Elastic Block Store (EBS)

## Parte 1: O que é o Amazon EBS?

### Definição Principal
O Amazon EBS fornece **volumes de armazenamento em bloco persistente** para uso com instâncias Amazon EC2. Armazenamento persistente (ou não volátil) é qualquer dispositivo de armazenamento que retém os dados mesmo após a energia ser desligada.

### Principais Características
* **Alta Disponibilidade e Durabilidade:** Cada volume EBS é automaticamente replicado dentro de sua Zona de Disponibilidade para protegê-lo contra falhas de componentes.
* **Desempenho:** Fornece o desempenho consistente e de baixa latência necessário para executar suas cargas de trabalho.
* **Escalabilidade:** Você pode escalar seu uso para mais ou para menos em questão de minutos, pagando um preço baixo apenas pelo que você provisiona.

---

## Parte 2: Conceito Chave - Armazenamento em Bloco vs. Armazenamento de Objetos

Uma diferença crucial entre os tipos de armazenamento é se eles oferecem armazenamento em bloco ou em nível de objeto.

> **Cenário:** O que acontece se você quiser mudar um único caractere em um arquivo de 1 Gigabyte?
> * **Com Armazenamento em Bloco (EBS):** Você altera **apenas o bloco** que contém o caractere.
> * **Com Armazenamento de Objetos (S3):** Você tem que **atualizar o arquivo inteiro**.

Essa diferença tem um grande efeito na taxa de transferência (throughput), na latência e no custo. Soluções de armazenamento em bloco são tipicamente mais rápidas e usam menos largura de banda, mas podem custar mais.

---

## Parte 3: Casos de Uso e Tipos de Volume

### Como é Usado na Prática?
Com o Amazon EBS, você pode criar volumes de armazenamento individuais e **anexá-los a uma instância Amazon EC2**. Por estarem diretamente anexados, eles fornecem baixa latência, o que torna o EBS uma excelente escolha para executar um banco de dados em uma instância EC2.

### Casos de Uso Típicos
* **Volumes de inicialização (boot)** e armazenamento para instâncias EC2.
* Um sistema de arquivos para armazenamento de dados.
* Hosts de banco de dados.
* Armazenamento para aplicações empresariais.
* Aplicações intensivas em taxa de transferência que realizam varreduras contínuas de disco.

### Tipos de Volume e Otimização de Custo
Você pode reduzir seus custos de armazenamento selecionando o tipo que melhor se adapta à sua carga de trabalho.
* **SSD de IOPS Provisionadas:** Oferece o mais alto desempenho.
* **SSD de Uso Geral:** Pode ser suficiente se sua aplicação não exigir um desempenho tão alto.
* **Outras opções de menor custo (HDD):** Podem ser uma solução para armazenamento adicional.
> **Nota Importante:** Apenas volumes do tipo **SSD** podem ser usados como volumes de inicialização para instâncias EC2.

---

## Parte 4: Funcionalidades Essenciais do EBS

### 1. Snapshots (Backups)
* **O que são?** Um backup de um volume EBS é chamado de snapshot. São "fotos" de um ponto no tempo de seus volumes.
* **Como Funcionam?** O primeiro snapshot é uma cópia completa (baseline). Os snapshots seguintes são incrementais, capturando apenas o que mudou desde o anterior.
* **Recuperação e Durabilidade:** Você pode recriar um novo volume a partir de um snapshot a qualquer momento. Você também pode compartilhar snapshots ou copiá-los para diferentes regiões da AWS para uma proteção ainda maior de recuperação de desastres (ex: da Virgínia para Tóquio).

### 2. Criptografia
* Você pode criptografar volumes Amazon EBS sem custo adicional, garantindo que os dados estejam seguros.

### 3. Elasticidade (Redimensionamento Dinâmico)
* Os volumes Amazon EBS podem ter sua capacidade aumentada e podem mudar para tipos diferentes.
* Você pode aumentar um volume de 50 GB para 16 TB, ou mudar de HDD para SSD.
* Esta operação de redimensionamento pode ser feita **dinamicamente, sem precisar parar as instâncias**.

---

## Parte 5: Entendendo os Custos do EBS

Aqui estão os componentes que formam o custo do Amazon EBS:

* **Armazenamento:** Para todos os tipos de volume, é cobrado pela quantidade que você provisiona em **Gigabytes por mês**, até que você libere o armazenamento.
* **Entrada/Saída (I/O):**
    * **SSD de Uso Geral:** O I/O está incluído no preço.
    * **Volumes Magnéticos:** O I/O é cobrado pelo número de solicitações que você faz ao volume.
    * **SSD de IOPS Provisionadas:** Você também é cobrado pela quantidade que provisiona em **IOPS** (operações de entrada/saída por segundo).
* **Snapshots:** O custo é por **Gigabyte por mês** que os dados são armazenados.
* **Cópia de Snapshots:** Ao copiar snapshots entre regiões, você é cobrado pelos dados transferidos. Após a cópia, aplicam-se as cobranças padrão de armazenamento de snapshot na região de destino.

# Como Criar e Gerenciar um Volume EBS (Guia Prático)

Este guia é um passo a passo baseado na demonstração de gerenciamento de um volume EBS com uma instância Linux.

## Parte 1: Conceitos e Preparação

### O que é um Volume EBS?
* É o equivalente a um **disco rígido** para uma instância EC2.
* Oferece **armazenamento em bloco persistente**, ou seja, os dados permanecem mesmo se a instância for parada.
* É um volume anexado pela rede, que persiste independentemente da vida da instância.
* Pode ser usado como **partição de inicialização (boot)**, o que permite que a instância seja parada e reiniciada.
* É altamente durável, pois é **replicado automaticamente** dentro de sua Zona de Disponibilidade.

### Preparação: O Ponto Mais Importante
> **Atenção:** Um volume EBS só pode ser anexado a uma instância EC2 que esteja na **mesma Zona de Disponibilidade (AZ)**. Antes de criar um volume, verifique a AZ da sua instância (ex: `us-west-2d`).

---

## Parte 2: Criação e Anexação de um Novo Volume

### Passo 1: Criar o Volume
1.  No Console da AWS, navegue até o serviço **EC2**.
2.  No menu à esquerda, em **Elastic Block Store**, clique em **Volumes**.
3.  Clique no botão **Criar Volume**.
4.  **Configure o Volume:**
    * **Tipo de Volume:** Selecione o tipo desejado (ex: `General Purpose GP2`). *Nota: Apenas volumes SSD (GP2, IO1) podem ser usados como volume de inicialização.*
    * **Tamanho:** Defina o tamanho em GiB (ex: `10`).
    * **Zona de Disponibilidade:** **Selecione a mesma AZ da sua instância EC2**.
    * **Snapshot ID:** Deixe em branco para criar um volume novo e vazio.
    * **Criptografia:** (Opcional) Marque para criptografar o volume.
    * **Tags:** Adicione uma tag `Name` para identificar o volume (ex: `EBS1`).
5.  Clique em **Criar Volume**.

### Passo 2: Anexar o Volume à Instância EC2
1.  Aguarde o **Estado** do novo volume mudar para `disponível`.
2.  Selecione o volume, clique em **Ações** > **Anexar Volume**.
3.  Na caixa de diálogo, no campo **Instância**, selecione a sua instância EC2 de destino.
4.  Anote o **Nome do dispositivo** que a AWS sugere (ex: `/dev/sdf`). Você precisará dele mais tarde.
5.  Clique em **Anexar**. O **Estado** do volume mudará para `em uso`.

---

## Parte 3: Formatação e Montagem do Volume (No Linux)

Mesmo anexado, o sistema operacional ainda não pode usar o volume. É preciso formatá-lo e montá-lo.

### Passo 3: Formatar o Volume com um Sistema de Arquivos
1.  Conecte-se à sua instância EC2 via SSH.
2.  Execute o comando para criar um sistema de arquivos. Use o nome do dispositivo que você anotou.
    ```bash
    sudo mkfs -t ext4 /dev/sdf
    ```

### Passo 4: Criar um Ponto de Montagem
1.  Crie um diretório que servirá como o "local" onde o volume será acessado.
    ```bash
    sudo mkdir /datastore
    ```

### Passo 5: Montar o Volume
1.  Execute o comando para "ligar" o dispositivo ao diretório.
    ```bash
    sudo mount /dev/sdf /datastore
    ```

### Passo 6: Verificar a Montagem
1.  Execute o comando `df -h` para listar os sistemas de arquivos montados. Você deverá ver seu novo volume de 10 GiB montado em `/datastore`.

---

## Parte 4: Backup e Restauração com Snapshots

### Passo 7: Criar um Snapshot
Snapshots são backups incrementais de seus volumes, armazenados de forma durável no Amazon S3.

1.  No console do EC2, vá para **Elastic Block Store** > **Snapshots**.
2.  Clique em **Criar Snapshot**.
3.  Em **Recurso**, selecione **Volume** e escolha o ID do volume que deseja copiar (ex: `EBS1`).
4.  Adicione uma **Descrição** e **Tags** para identificar o snapshot (ex: `Name: EBS2`).
5.  Clique em **Criar Snapshot**.

### Passo 8: Restaurar o Snapshot para um Novo Volume (com Redimensionamento)
1.  Aguarde o status do snapshot mudar para `concluído`.
2.  Selecione o snapshot, clique em **Ações** > **Criar Volume a partir do snapshot**.
3.  Na tela de criação, você pode modificar as configurações. Por exemplo, aumente o **Tamanho** para `15` GiB.
4.  **CRÍTICO:** Certifique-se de que a **Zona de Disponibilidade** é a mesma da sua instância EC2.
5.  Dê um nome ao novo volume (ex: `restored-volume`) e clique em **Criar Volume**.
6.  Após a criação, **anexe** este novo volume à sua instância EC2, como fez no Passo 2.

---

## Parte 5: Estendendo o Sistema de Arquivos (No Linux)

### Passo 9: Reconhecer o Novo Tamanho no Sistema Operacional
O volume agora tem 15 GiB, mas o sistema de arquivos dentro dele ainda pensa que tem 10 GiB. É preciso estendê-lo.

> **Boa Prática:** Antes de estender um sistema de arquivos com dados valiosos, crie um snapshot para o caso de precisar reverter as alterações.

1.  Conectado à instância, use `lsblk` para ver os volumes e seus tamanhos.
2.  Use o comando `resize2fs` para redimensionar o sistema de arquivos. Use o nome do dispositivo do novo volume.
    ```bash
    sudo resize2fs /dev/sdg
    ```
    *(O nome do dispositivo pode variar, use o que foi mostrado ao anexar).*

### Passo 10: Verificar o Resultado e os Dados
1.  Execute `df -h` novamente. O tamanho do volume montado agora deve refletir os 15 GiB.
2.  Se você tinha dados no volume original quando tirou o snapshot, eles estarão no volume restaurado. Verifique listando os arquivos:
    ```bash
    ls /caminho/de/montagem/do/volume/restaurado
    ```

# Guia Completo do Amazon Simple Storage Service (S3)

## Parte 1: Conceitos Fundamentais do S3

### O que é Armazenamento de Objetos?
O Amazon S3 é um serviço de **armazenamento em nível de objeto**. Isso significa que, se você quiser alterar uma parte de um arquivo, deve fazer a alteração e, em seguida, **reenviar o arquivo modificado inteiro**.

### Estrutura Básica
* **Objetos:** Os dados são armazenados como objetos, que podem ser quase qualquer tipo de arquivo (imagens, vídeos, logs, etc.).
* **Buckets:** Os objetos são armazenados em recursos chamados buckets.

### Principais Características
* **Solução Gerenciada:** Você não precisa gerenciar nenhuma infraestrutura. O S3 escala perfeitamente e lida com um volume massivo de requisições.
* **Durabilidade:** Projetado para fornecer **onze noves (99,999999999%) de durabilidade**.
* **Escala:** Você pode armazenar uma quantidade virtualmente ilimitada de objetos em um bucket, com objetos individuais podendo ter até 5 terabytes de tamanho.
* **Nomenclatura:** Os nomes dos buckets são universais e devem ser **únicos em todo o mundo**.

---

## Parte 2: Segurança e Funcionalidades

### Controle de Acesso e Segurança
* **Controle Granular:** Você pode controlar quem pode acessar seus dados usando:
    * Políticas do AWS IAM.
    * Políticas de Bucket do S3.
    * Listas de Controle de Acesso (ACLs) por objeto.
* **Privacidade Padrão:** Por padrão, nenhum de seus dados é compartilhado publicamente.
* **Criptografia:** Você pode criptografar seus dados em trânsito e em repouso ativando a criptografia do lado do servidor.

### Notificações de Eventos
* O S3 permite configurar notificações automáticas quando certos eventos ocorrem (ex: um objeto é carregado ou excluído).
* Essas notificações podem ser enviadas a você ou usadas para acionar outros processos, como funções do **AWS Lambda**.

---

## Parte 3: As Classes de Armazenamento do S3

O S3 oferece uma gama de classes de armazenamento projetadas para diferentes casos de uso.

| Classe de Armazenamento | Ideal Para (Caso de Uso) | Principais Características |
| :--- | :--- | :--- |
| **S3 Standard** | Dados acessados com frequência, distribuição de conteúdo, análise de big data. | Alta disponibilidade, durabilidade e desempenho; baixa latência e alta taxa de transferência. |
| **S3 Standard-IA** | Dados acessados com menos frequência, mas que exigem acesso rápido quando necessário; armazenamento de longo prazo, backups, recuperação de desastres. | Mesma durabilidade, taxa de transferência e baixa latência do Standard, com um preço de armazenamento por GB mais baixo, mas com uma taxa de recuperação por GB. |
| **S3 One Zone-IA** | Dados acessados com pouca frequência que não exigem a resiliência de múltiplas AZs; cópias de backup secundárias, dados fáceis de recriar (ex: thumbnails). | Armazena dados em uma **única Zona de Disponibilidade**. Custa menos que o Standard-IA. |
| **S3 Intelligent-Tiering**| Dados de longa duração com padrões de acesso desconhecidos, imprevisíveis ou variáveis. | Move automaticamente os dados entre as camadas de acesso frequente e infrequente para otimizar custos. Cobra uma pequena taxa de monitoramento por objeto. |
| **S3 Glacier** | Arquivamento de dados de longo prazo. | Custo de armazenamento muito baixo. Oferece três opções de recuperação que variam de **alguns minutos a horas**. |
| **S3 Glacier Deep Archive**| Retenção de longo prazo (7-10 anos) e preservação digital para dados acessados uma ou duas vezes por ano; setores regulamentados (financeiro, saúde); alternativa para sistemas de fita magnética. | A classe de armazenamento de **menor custo**. Os objetos podem ser restaurados em até **12 horas**. |

---

## Parte 4: Buckets em Profundidade

### O que são?
* Buckets são contêineres lógicos para objetos. Você pode ter um ou mais buckets em sua conta e controlar quem pode criar, deletar e listar objetos neles.

### Regionalidade e Redundância
* Quando você cria um bucket, ele é associado a uma **Região AWS** específica.
* Os dados armazenados no bucket são **redundantemente armazenados em múltiplas instalações da AWS dentro daquela região selecionada**.

### Regras de Nomenclatura
* Devem ser **globalmente únicos**.
* Devem ser compatíveis com DNS: tudo em **letras minúsculas**, contendo apenas uma combinação de letras, números e hífens.

### Formatos de URL
* **URL no Estilo de Caminho (Path-style):** Usada normalmente para acessar objetos. Ex: `s3.region.amazonaws.com/nome-do-bucket/objeto.jpg`
* **URL no Estilo de Hospedagem Virtual (Virtual-hosted style):** Usada quando você está usando seu bucket como um site para dados estáticos. Ex: `nome-do-bucket.s3.region.amazonaws.com/objeto.jpg`

---

## Parte 5: Casos de Uso e Custos

### Casos de Uso Comuns
* **Hospedagem de sites estáticos:** Servir o conteúdo estático do seu site (HTML, CSS, JavaScript, etc.).
* **Backups:** A alta durabilidade do S3 o torna um ótimo candidato para armazenar backups.
* **Replicação entre regiões (Cross-Region Replication):** Para maior disponibilidade e capacidade de recuperação de desastres, o S3 pode ser configurado para replicar dados automaticamente para um bucket em outra região.

### Entendendo os Custos do S3
Você paga apenas pelo que usa. Os custos variam por região e são compostos por:
* **Armazenamento:** Cobrado em Gigabytes por mês (as taxas variam por classe de armazenamento).
* **Requisições:** Solicitações como `PUT`, `COPY`, `POST`, `LIST` e `GET` incorrem em cobranças com taxas diferentes.
* **Transferência de Dados:**
    * Transferência de dados **PARA DENTRO** do S3 é geralmente gratuita.
    * Transferência de dados **PARA FORA** do S3 é cobrada (com exceção da transferência para o Amazon CloudFront na mesma região).

# Guia do Amazon Elastic File System (EFS)

## Parte 1: O que é o Amazon EFS?

### Definição Principal
O Amazon EFS implementa um tipo de armazenamento para instâncias EC2 que **múltiplas máquinas virtuais podem acessar ao mesmo tempo**.

* **Analogia:** Pense no EFS como um **armazenamento de arquivos na nuvem** (semelhante a um "servidor de arquivos" ou "drive de rede").
* **Tecnologia:** É implementado como um **sistema de arquivos compartilhado** que utiliza o protocolo **Network File System (NFS)** (versões 4.0 e 4.1).

### Principais Características e Benefícios
* **Serviço Totalmente Gerenciado:** Facilita a configuração e o escalonamento do armazenamento de arquivos.
* **Semântica de Acesso Completa:** Suporta funcionalidades de sistema de arquivos tradicionais, como **consistência forte** e **bloqueio de arquivos (file locking)**.
* **Escalabilidade Automática:** Escala de gigabytes para petabytes de dados automaticamente, sem a necessidade de provisionar o armazenamento previamente.
* **Acesso Concorrente:** Milhares de instâncias EC2 podem acessar um sistema de arquivos EFS simultaneamente.
* **Desempenho Consistente:** Fornece desempenho consistente para cada instância EC2 conectada.
* **Alta Durabilidade e Disponibilidade.**
* **Modelo de Preços:** Não há taxa mínima ou custos de configuração. **Você paga apenas pelo armazenamento que usa**.

---

## Parte 2: Casos de Uso Comuns
O EFS é ideal para cenários que exigem um sistema de arquivos compartilhado, como:
* Big data e analytics
* Fluxos de trabalho de processamento de mídia
* Gerenciamento de conteúdo
* Serviço web (web serving)
* Diretórios home compartilhados

---

## Parte 3: Como o EFS Funciona - Montagem e Acesso

O processo geral é criar um sistema de arquivos, montá-lo em uma instância EC2 e, em seguida, ler e escrever dados nele.

### Acesso Dentro da VPC
* Você pode montar um sistema de arquivos EFS em sua VPC.
* A principal vantagem é que instâncias EC2 rodando em **múltiplas Zonas de Disponibilidade**, dentro da mesma Região AWS, podem acessar o sistema de arquivos. Isso permite que muitos usuários e aplicações compartilhem uma fonte de dados comum.

### Destinos de Montagem (Mount Targets)
* Para que as instâncias EC2 em uma sub-rede da sua VPC acessem o sistema de arquivos, você cria um **destino de montagem** naquela sub-rede.
* O destino de montagem fornece um "ponto de acesso" ao sistema de arquivos EFS a partir daquela Zona de Disponibilidade específica.
* **Recomendação:** Acesse o sistema de arquivos a partir de um destino de montagem que esteja na mesma Zona de Disponibilidade da sua instância EC2 para obter a melhor performance.

---

## Parte 4: Os 5 Passos para Configurar o EFS
1.  **Crie seus recursos EC2:** Lance as instâncias que precisarão acessar o sistema de arquivos.
2.  **Crie seu sistema de arquivos EFS:** Crie o recurso primário do EFS no console.
3.  **Crie seus destinos de montagem:** Crie os destinos de montagem nas sub-redes apropriadas (nas AZs onde suas instâncias EC2 estão).
4.  **Conecte e monte:** Conecte-se à sua instância EC2 e use os comandos do Linux para montar o sistema de arquivos EFS.
5.  **Limpe seus recursos:** Ao final, lembre-se de deletar os recursos para não incorrer em custos.

---

## Parte 5: Recursos e Metadados
* **Recurso Primário:** O **Sistema de Arquivos**, com suas propriedades (ID, tempo de criação, tamanho, etc.).
* **Sub-recursos:**
    * **Destinos de Montagem:** Não existem sem estarem associados a um sistema de arquivos e a uma sub-rede.
    * **Tags:** Pares chave-valor que você pode atribuir aos seus sistemas de arquivos para organizá-los.

# Guia Detalhado do Amazon S3 Glacier e Criptografia no S3

## Parte 1: O que é o Amazon S3 Glacier?

### Definição Principal
O Amazon S3 Glacier é um serviço de armazenamento em nuvem seguro, durável e de **custo extremamente baixo**, ideal para **arquivamento de dados e backup de longo prazo**.

A principal característica é o equilíbrio entre custo e tempo de acesso: o custo de armazenamento é muito baixo, mas a recuperação dos dados não é imediata e pode levar várias horas.

### Os 3 Termos-Chave do Glacier
1.  **Arquivo (Archive):** É a unidade base de armazenamento no Glacier. Pode ser qualquer objeto, como uma foto, vídeo ou documento.
2.  **Cofre (Vault):** É um contêiner para armazenar os arquivos. Ao criar um cofre, você especifica um nome e a Região AWS.
3.  **Políticas de Cofre:**
    * **Política de Acesso ao Cofre:** Determina quem pode (e não pode) acessar os dados e quais operações podem ser realizadas.
    * **Política de Bloqueio de Cofre (Vault Lock):** Pode ser usada para aplicar controles de conformidade e garantir que um cofre não possa ser alterado (política de imutabilidade).

### As 3 Opções de Recuperação de Dados
| Tipo de Recuperação | Tempo Típico | Custo |
| :--- | :--- | :--- |
| **Acelerada (Expedited)** | 1 a 5 minutos | O mais alto |
| **Padrão (Standard)** | 3 a 5 horas | Intermediário |
| **em Massa (Bulk)** | 5 a 12 horas | O mais baixo |

---

## Parte 2: Casos de Uso e Interação com o Serviço

### Casos de Uso Comuns
* Arquivamento de ativos de mídia (vídeos, notícias).
* Arquivamento de informações de saúde (registros de pacientes por décadas).
* Arquivamento para conformidade e regulamentação (serviços financeiros).
* Arquivamento de dados científicos.
* Preservação digital (bibliotecas, agências governamentais).
* Alternativa para sistemas de **fita magnética**, sem custo inicial e com menor manutenção.

### Como Interagir com o Glacier
* **Console da AWS:** Permite apenas operações limitadas, como criar/excluir cofres e gerenciar políticas.
* **Acesso Programático (para a maioria das operações):** É necessário usar as APIs REST do Glacier, os SDKs da AWS (Java, .NET) ou a AWS CLI.

---

## Parte 3: S3 e Glacier - A Relação via Ciclo de Vida

Você pode usar **Políticas de Ciclo de Vida** para automatizar a movimentação de dados entre as diferentes classes de armazenamento do S3 e, finalmente, para o Glacier, reduzindo custos à medida que os dados envelhecem.

* **Exemplo:** Um thumbnail de vídeo é carregado no `S3 Standard`. Após 30 dias sem acesso, uma política de ciclo de vida o move para `S3 Standard-IA`. Após mais 30 dias, ele é movido para o `S3 Glacier`. Depois de um ano, ele é excluído. A política gerencia tudo isso automaticamente.

---

## Parte 4: Revisão de Todas as Classes de Armazenamento do S3
* **S3 Standard:** Para dados acessados com frequência e sensíveis ao desempenho.
* **S3 Intelligent-Tiering:** Otimiza custos movendo dados automaticamente entre as camadas de acesso frequente e infrequente.
* **S3 Standard-Infrequent Access (Standard-IA):** Para dados de longa duração, acessados com menos frequência, mas que ainda exigem alto desempenho quando acessados.
* **S3 One Zone-Infrequent Access (One Zone-IA):** Armazena dados em uma única AZ, com custo menor que o Standard-IA.
* **S3 Glacier:** Para arquivamento de dados onde o acesso é infrequente e um tempo de recuperação de várias horas é aceitável.
* **S3 Glacier Deep Archive:** A classe de menor custo, para retenção de longo prazo (7-10 anos) de dados acessados uma ou duas vezes por ano.

---

## Parte 5: Comparação Detalhada - S3 Standard vs. S3 Glacier

| Característica | Amazon S3 (Standard) | Amazon S3 Glacier |
| :--- | :--- | :--- |
| **Caso de Uso Principal**| Acesso frequente e de baixa latência | Armazenamento de longo prazo, de baixo custo e acesso infrequente |
| **Custo** | Custo de armazenamento por GB mais alto; custo de recuperação mais baixo | Custo de armazenamento por GB muito mais baixo; custo de recuperação mais alto |
| **Tamanho Máximo do Objeto**| 5 TB | 40 TB |
| **Cobrança de Requisições**| `PUT`, `COPY`, `POST`, `LIST`, `GET` | Upload e Recuperação |
| **Criptografia Padrão**| **Não** é criptografado por padrão (a aplicação deve iniciar) | **Sim**, os dados são criptografados por padrão |

---

## Parte 6: Aprofundando na Criptografia do Lado do Servidor (SSE) no S3

Existem três maneiras de habilitar a criptografia do lado do servidor para proteger dados em repouso no S3:

#### 1. SSE-S3: Chaves Gerenciadas pelo S3
* O Amazon S3 gerencia as chaves de criptografia.
* Cada objeto é criptografado com uma chave única, que por sua vez é criptografada com uma chave mestra que o S3 rotaciona regularmente. Utiliza o robusto cifrador **AES-256**.

#### 2. SSE-C: Chaves Fornecidas pelo Cliente
* Você fornece sua própria chave de criptografia junto com cada requisição de objeto.
* O S3 usa sua chave para criptografar (ao salvar) e descriptografar (ao acessar) os dados, mas **não armazena sua chave**.

#### 3. SSE-KMS: Chaves Gerenciadas pelo AWS Key Management Service (KMS)
* Usa o serviço AWS KMS para gerenciar as chaves mestras (CMKs) que criptografam seus objetos S3.
* Permite **criar e gerenciar chaves de forma centralizada**, definir políticas de controle de uso e auditar o uso das chaves para fins de conformidade.

---

## Parte 7: Resumo da Segurança no Glacier
O Glacier aplica duas camadas de segurança:
1.  **Controle de Acesso:** Você controla o acesso aos seus dados usando o **IAM**.
2.  **Criptografia:** Seus dados são **criptografados por padrão**, e você pode escolher como gerenciar as chaves.

# Módulo de Armazenamento: Revisão Final e Questão Prática

## Checklist de Aprendizagem do Módulo
Ao concluir este módulo, você aprendeu a:

* Identificar os diferentes tipos de armazenamento (Objetos, Blocos, Arquivos).
* Explicar e descrever a funcionalidade do Amazon S3, Amazon EBS, Amazon EFS e Amazon S3 Glacier.
* Entender os diferentes casos de uso para esses serviços e como escolher a solução de armazenamento correta com base em seus requisitos.

---

## Análise de Questão Prática (Exemplo de Exame)

### A Pergunta

> "Uma empresa quer armazenar dados que não são acessados com frequência. Qual é a melhor e mais econômica solução que deve ser considerada?"

### Análise das Palavras-Chave

* **"Não são acessados com frequência":** Esta é a principal característica do padrão de acesso dos dados.
* **"Solução econômica":** Este é o principal requisito de negócio.

### A Resposta Correta e a Justificativa

Com base nas palavras-chave, a resposta correta é **B, Amazon S3 Glacier**.

O Glacier é a maneira mais econômica de armazenar dados que não são acessados com frequência.
