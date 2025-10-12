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

# Módulo 9: Arquitetura na Nuvem (Guia Completo do Well-Architected Framework)

## Parte 1: Introdução ao AWS Well-Architected Framework

### O que é Arquitetura e o Papel do Arquiteto de Nuvem?
* **Arquitetura:** É a arte e a ciência de projetar e construir grandes estruturas. Sistemas grandes requerem arquitetos para gerenciar seu tamanho e complexidade.
* **O que fazem os arquitetos de nuvem?**
    1.  Engajam-se com os tomadores de decisão para identificar o objetivo de negócio e as capacidades que precisam de melhoria.
    2.  Garantem o alinhamento entre os entregáveis de tecnologia de uma solução e as metas de negócio.
    3.  Trabalham com as equipes de entrega para garantir que os recursos tecnológicos sejam apropriados.

### O que é o AWS Well-Architected Framework?
É um guia projetado para ajudá-lo a construir a infraestrutura **mais segura, de alto desempenho, resiliente e eficiente** possível para suas aplicações e cargas de trabalho na nuvem.
* Ele fornece um conjunto de perguntas fundamentais e as melhores práticas que podem ajudá-lo a avaliar e implementar suas arquiteturas.
* Foi desenvolvido pela AWS após a revisão de milhares de arquiteturas de clientes.

### Como o Framework é Organizado?
O framework é organizado em **cinco pilares**. Cada pilar inclui um conjunto de princípios de design e melhores práticas.

---

## Parte 2: Os 5 Pilares do Well-Architected Framework

### 1. Pilar de Excelência Operacional
* **Foco:** A capacidade de executar e monitorar sistemas para entregar valor de negócio e melhorar continuamente as operações.
* **Tópicos-chave:** Gerenciar e automatizar mudanças, responder a eventos e definir padrões para gerenciar com sucesso as operações diárias.

#### Princípios de Design (6)
1.  **Executar operações como código:** Defina toda a sua carga de trabalho (aplicação e infraestrutura) como código para limitar o erro humano e permitir respostas consistentes a eventos.
2.  **Anotar documentação:** Automatize a criação de documentação anotada após cada build.
3.  **Fazer mudanças pequenas, frequentes e reversíveis:** Projete componentes para serem atualizados regularmente em pequenos incrementos que podem ser revertidos se falharem.
4.  **Refinar procedimentos operacionais frequentemente:** Procure oportunidades para melhorar e atualizar os procedimentos à medida que evoluem.
5.  **Antecipar falhas:** Identifique fontes potenciais de falha para que possam ser removidas ou mitigadas. Teste cenários de falha regularmente.
6.  **Aprender com todos os eventos e falhas operacionais:** Compartilhe o que foi aprendido entre as equipes e em toda a organização.

### 2. Pilar de Segurança
* **Foco:** A capacidade de proteger informações, sistemas e ativos, entregando valor de negócio através de avaliação de riscos e estratégias de mitigação.
* **Tópicos-chave:** Proteger a confidencialidade e integridade dos dados, gerenciar privilégios, proteger sistemas e detectar eventos de segurança.

#### Princípios de Design (7)
1.  **Implementar uma base de identidade forte:** Implemente o princípio do menor privilégio e a separação de deveres.
2.  **Habilitar a rastreabilidade:** Monitore, alerte e audite ações e mudanças em seu ambiente em tempo real.
3.  **Aplicar segurança em todas as camadas:** Aplique defesa em profundidade e controles de segurança em todas as camadas da sua arquitetura (rede de borda, VPC, sub-rede, load balancer, instância, SO, aplicação).
4.  **Automatizar as melhores práticas de segurança:** Automatize mecanismos de segurança para escalar de forma mais rápida e econômica.
5.  **Proteger dados em trânsito e em repouso:** Classifique seus dados e use mecanismos como criptografia, tokenização e controle de acesso.
6.  **Manter as pessoas longe dos dados:** Crie mecanismos e ferramentas para reduzir ou eliminar a necessidade de acesso direto ou processamento manual de dados sensíveis.
7.  **Preparar-se para eventos de segurança:** Tenha um processo de gerenciamento de incidentes e execute simulações de resposta a incidentes.

### 3. Pilar de Confiabilidade
* **Foco:** A capacidade de um sistema se recuperar de interrupções, adquirir dinamicamente recursos para atender à demanda e mitigar interrupções (como erros de configuração ou problemas de rede).
* **Tópicos-chave:** Configuração, planejamento de recuperação e gerenciamento de mudanças.

#### Princípios de Design (5)
1.  **Testar procedimentos de recuperação:** Teste como seus sistemas falham e valide seus procedimentos de recuperação para expor falhas antes que elas aconteçam de verdade.
2.  **Recuperar-se automaticamente de falhas:** Monitore sistemas por KPIs (Key Performance Indicators) e configure-os para acionar uma recuperação automatizada quando um limiar for violado.
3.  **Escalar horizontalmente para aumentar a disponibilidade agregada:** Substitua um recurso grande por múltiplos recursos menores para reduzir o impacto de um único ponto de falha.
4.  **Parar de adivinhar a capacidade:** Monitore a demanda e o uso do sistema e automatize a adição ou remoção de recursos para manter o nível ideal.
5.  **Gerenciar mudanças na automação:** Use automação para fazer e gerenciar mudanças na infraestrutura.

### 4. Pilar de Eficiência de Performance
* **Foco:** A capacidade de usar recursos de TI e computação de forma eficiente para atender aos requisitos do sistema e manter essa eficiência à medida que as demandas ou tecnologias mudam.
* **Tópicos-chave:** Selecionar os tipos e tamanhos de recursos corretos, monitorar o desempenho e tomar decisões informadas para manter a eficiência.

#### Princípios de Design (5)
1.  **Democratizar tecnologias avançadas:** Consuma tecnologias complexas (NoSQL, machine learning, etc.) como um serviço, permitindo que as equipes foquem no desenvolvimento do produto.
2.  **Tornar-se global em minutos:** Implante sistemas em múltiplas regiões da AWS para fornecer menor latência e uma melhor experiência ao cliente a um custo mínimo.
3.  **Usar arquiteturas sem servidor (serverless):** Remova o fardo operacional de executar e manter servidores.
4.  **Experimentar mais frequentemente:** Realize testes comparativos de diferentes tipos de instâncias, armazenamento ou configurações.
5.  **Ter simpatia mecânica:** Use a abordagem tecnológica que melhor se alinha ao que você está tentando alcançar (ex: considere seus padrões de acesso a dados ao selecionar um banco de dados).

### 5. Pilar de Otimização de Custos
* **Foco:** A capacidade de executar sistemas para entregar valor de negócio ao menor preço possível.
* **Tópicos-chave:** Entender e controlar onde o dinheiro está sendo gasto, selecionar os recursos apropriados, analisar gastos ao longo do tempo e escalar sem gastar demais.

#### Princípios de Design (5)
1.  **Adotar um modelo de consumo:** Pague apenas pelos recursos de computação que você precisa, aumentando ou diminuindo o uso com base nos requisitos de negócio, não em previsões elaboradas.
2.  **Medir a eficiência geral:** Meça o resultado de negócio da carga de trabalho e os custos associados a ele.
3.  **Parar de gastar dinheiro em operações de data center:** Deixe a AWS cuidar do trabalho pesado de empilhar e alimentar servidores, para que você possa focar em seus clientes e projetos de negócio.
4.  **Analisar e atribuir despesas:** Identifique o uso e os custos do sistema e atribua os custos de TI a proprietários individuais de cargas de trabalho.
5.  **Usar serviços gerenciados e de nível de aplicação para reduzir o custo de propriedade:** Eles reduzem o fardo operacional e podem oferecer um custo menor por transação.

---

## Parte 3: Aprofundando em Confiabilidade e Alta Disponibilidade

> "Tudo falha o tempo todo." - Werner Vogels, CTO da Amazon

* **Confiabilidade:** É a probabilidade de um sistema inteiro (hardware, firmware, software) funcionar como pretendido por um período especificado. É medida estatisticamente.
    * **Tempo Médio Entre Falhas (MTBF):** É a soma do Tempo Médio Para Falhar (MTTF) e o Tempo Médio Para Reparar (MTTR). No exemplo dado: `MTBF = 96h (MTTF) + 72h (MTTR) = 168h (1 semana)`.

* **Disponibilidade:** É a porcentagem de tempo que um sistema está operando normalmente. É comumente definida como a porcentagem de tempo de atividade (uptime) em um período (geralmente um ano). Uma forma abreviada de se referir à disponibilidade é o **número de "noves"** (ex: "cinco noves" = 99,999%).

* **Alta Disponibilidade:** Um sistema altamente disponível pode suportar alguma degradação enquanto permanece disponível, com tempo de inatividade minimizado e mínima intervenção humana.

* **Fatores que Determinam a Disponibilidade:**
    1.  **Tolerância a falhas:** A redundância embutida dos componentes de uma aplicação.
    2.  **Escalabilidade:** A capacidade da aplicação de acomodar aumentos de capacidade.
    3.  **Recuperabilidade:** A capacidade de restaurar o serviço rapidamente e sem perda de dados.

> **Equilíbrio Custo-Benefício:** Lembre-se que melhorar a disponibilidade geralmente leva a um aumento de custo. É importante equilibrar o custo da melhoria com o benefício para seus usuários.

---

## Parte 4: AWS Trusted Advisor - A Ferramenta de Análise
O Trusted Advisor analisa todo o seu ambiente AWS e fornece recomendações em cinco categorias para ajudá-lo a seguir as melhores práticas.

#### As 5 Categorias de Recomendações:
1.  **Otimização de Custos:** Recomendações para otimizar custos, como eliminar recursos ociosos ou não utilizados e se comprometer com capacidade reservada.
2.  **Performance:** Recomendações para melhorar o desempenho, verificando limites de serviço, taxa de transferência provisionada e monitorando instâncias superutilizadas.
3.  **Segurança:** Recomendações para melhorar a segurança, identificando lacunas, recursos de segurança a serem habilitados e examinando permissões.
4.  **Tolerância a Falhas:** Recomendações para aumentar a disponibilidade e redundância, aproveitando o auto scaling, health checks, implantações Multi-AZ e backups.
5.  **Limites de Serviço:** Verifica o uso de serviços que está acima de 80% do limite do serviço.

> **Quando Usar?** Você não precisa esperar ter um ambiente de produção pronto. Pode usar o Trusted Advisor assim que começar a implementar suas arquiteturas.

---

## Parte 5: Revisão Final e Questão Prática do Módulo

### Checklist de Aprendizagem do Módulo
* Descrever o AWS Well-Architected Framework, incluindo os cinco pilares.
* Identificar os princípios de design do framework.
* Explicar a importância da confiabilidade e alta disponibilidade.
* Identificar como o AWS Trusted Advisor ajuda os clientes e interpretar suas recomendações.

### Análise de Questão Prática
* **A Pergunta:** "Um engenheiro de SysOps quer proteger seus dados em trânsito e em repouso. Que serviços ele poderia usar para proteger seus dados?"
* **As Palavras-Chave:** "Proteger seus dados em trânsito e em repouso".
* **A Resposta Correta e a Justificativa:** A resposta correta é **D, todos os anteriores**. Elastic Load Balancing, Amazon EBS e Amazon S3 incluem capacidades de criptografia para proteger dados em trânsito e em repouso.
