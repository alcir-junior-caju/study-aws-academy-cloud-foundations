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

# Módulo 10: Escalabilidade Automática e Monitoramento (Guia Completo)

## Parte 1: Introdução ao Módulo
Este módulo aborda três serviços que, embora funcionem bem individualmente, tornam-se ainda mais poderosos quando usados em conjunto:
* Elastic Load Balancing (ELB)
* Amazon CloudWatch
* Amazon EC2 Auto Scaling

Ao final do módulo, você será capaz de distribuir tráfego (ELB), monitorar recursos (CloudWatch) e escalar servidores automaticamente (Auto Scaling) para melhorar uma arquitetura.

---

## Parte 2: Guia do Elastic Load Balancing (ELB)

### O Problema que Resolve
Sites modernos de alto tráfego precisam servir milhões de requisições simultâneas. Para atender a essa demanda, são necessários servidores adicionais, e o tráfego precisa ser distribuído entre eles de forma eficiente.

### O que é?
O ELB é um serviço que **distribui o tráfego de entrada** da aplicação ou da rede entre múltiplos alvos, como instâncias EC2, contêineres, endereços IP e funções Lambda. Ele escala o balanceador de carga automaticamente conforme o tráfego muda.

### Os 3 Tipos de Load Balancer
| Tipo | Nível OSI | Roteamento Baseado em | Ideal para |
| :--- | :--- | :--- | :--- |
| **Application Load Balancer (ALB)** | Camada 7 (Aplicação) | Conteúdo da requisição (HTTP/HTTPS) | Balanceamento de carga avançado de tráfego HTTP/HTTPS, microserviços, contêineres. |
| **Network Load Balancer (NLB)** | Camada 4 (Transporte) | Dados do protocolo IP (TCP/UDP) | Balanceamento de carga de tráfego TCP/UDP, altíssima performance (milhões de req/s) e padrões de tráfego voláteis. |
| **Classic Load Balancer (CLB)** | Camada 7 e 4 | Requisição ou Conexão | Aplicações legadas. A AWS recomenda o uso de ALB ou NLB quando possível. |

### Como Funciona?
* **Listeners:** São processos que verificam por requisições de conexão. Cada listener é configurado com um protocolo (ex: HTTP) e uma porta (ex: 80) para o tráfego que vem dos clientes.
* **Grupos de Alvos (Target Groups):** Com ALBs e NLBs, você registra seus alvos (ex: instâncias EC2) em grupos e roteia o tráfego para esses grupos. Com CLBs, você registra as instâncias diretamente.
* **Verificações de Saúde (Health Checks):** O balanceador monitora a saúde dos alvos registrados e envia tráfego apenas para as instâncias saudáveis. Se um alvo fica doente, o tráfego é interrompido até que ele se recupere.

### Casos de Uso Comuns
* **Alta Disponibilidade e Tolerância a Falhas:** Balanceia o tráfego entre alvos saudáveis em múltiplas Zonas de Disponibilidade.
* **Suporte a Contêineres:** Um balanceador de carga pode distribuir o tráfego entre múltiplos contêineres rodando em diferentes portas na mesma instância EC2, com integração profunda com o Amazon ECS.

### Monitoramento
* **Amazon CloudWatch Metrics:** O ELB publica métricas sobre seus balanceadores e alvos.
* **Logs de Acesso:** Capturam informações detalhadas sobre cada requisição e as armazenam no S3 para análise.
* **AWS CloudTrail:** Captura todas as chamadas de API feitas ao serviço ELB para auditoria.

---

## Parte 3: Guia do Amazon CloudWatch

### O que é?
O CloudWatch é um serviço de **monitoramento e observabilidade** construído para engenheiros DevOps, desenvolvedores e gerentes de TI. Ele monitora seus recursos e aplicações da AWS em tempo real.

### Componentes e Funcionalidades Principais

#### 1. Métricas e Alarmes
* **Métricas:** São variáveis que você pode medir para seus recursos e aplicações (ex: utilização de CPU, latência de requisição, etc.).
* **Alarmes:** Você pode criar um alarme para monitorar qualquer métrica. Quando a métrica ultrapassa um limiar que você define, o alarme é acionado.
* **Ações de Alarme:** Um alarme pode:
    * Enviar uma notificação para o **Amazon Simple Notification Service (SNS)**.
    * Executar uma ação do **Amazon EC2 Auto Scaling**.
    * Executar uma ação direta do EC2 (parar, terminar, reiniciar).

#### 2. CloudWatch Events (Eventos)
* Permite definir regras que correspondem a eventos ou mudanças no seu ambiente AWS (ex: uma instância EC2 mudou de estado).
* Quando um evento corresponde a uma regra, ele pode ser roteado para alvos para processamento (ex: invocar uma função Lambda, iniciar uma tarefa ECS, etc.).

#### Como Configurar um Alarme (Baseado em Limiar Estático)
1.  **Namespace:** O serviço da AWS de onde a métrica vem (ex: `AWS/EC2`).
2.  **Métrica:** A variável que você quer medir (ex: `CPUUtilization`).
3.  **Estatística:** Como agregar a métrica (ex: Média, Mínima, Máxima).
4.  **Período:** O período de avaliação do alarme (ex: 5 minutos).
5.  **Condições:** O limiar para o alarme (ex: `> 80%`).
6.  **Configuração Adicional:** Quantos pontos de dados precisam violar o limiar para o alarme disparar.
7.  **Ação:** O que fazer quando o alarme disparar (enviar notificação, escalar, etc.).

---

## Parte 4: Guia do Amazon EC2 Auto Scaling

### O Problema que Resolve
Escalabilidade é a habilidade de aumentar ou diminuir a capacidade de computação. Provisionar capacidade fixa para o pico de demanda gera custos desnecessários (recursos ociosos), enquanto provisionar pouca capacidade causa problemas de performance e disponibilidade.

### O que é?
O EC2 Auto Scaling é um serviço que ajuda a manter a disponibilidade da aplicação e permite **adicionar (scale-out) ou remover (scale-in) instâncias EC2 automaticamente** de acordo com condições que você define.

### Componentes Principais
* **Grupo de Auto Scaling:** Uma coleção de instâncias EC2 tratadas como um agrupamento lógico. É definido por:
    * **Mínimo:** O número mínimo de instâncias que o grupo deve ter.
    * **Máximo:** O número máximo de instâncias que o grupo pode atingir.
    * **Capacidade Desejada:** O número de instâncias que o grupo deve ter em condições normais.
* **Configuração de Lançamento (Launch Configuration):** Um modelo de configuração de instância que o Auto Scaling usa para lançar novas instâncias (especificando AMI, tipo de instância, IAM Role, Security Groups, etc.).

### As Várias Maneiras de Escalar
* **Manter o Nível Atual:** O Auto Scaling realiza verificações de saúde e substitui automaticamente instâncias não saudáveis para manter a capacidade desejada.
* **Escalabilidade Manual:** Você altera manualmente a capacidade desejada do grupo.
* **Escalabilidade Agendada:** Ações de escalonamento são executadas em datas e horários pré-definidos. Ideal para cargas de trabalho previsíveis.
* **Escalabilidade Dinâmica (On-Demand):** A forma mais comum. Usa políticas de escalonamento que respondem a mudanças na demanda, geralmente acionadas por alarmes do CloudWatch.
* **Escalabilidade Preditiva:** Usa machine learning com base em dados históricos para prever a demanda futura e programar mudanças de capacidade com antecedência.

### Como os 3 Serviços Trabalham Juntos (Arquitetura Clássica)
1.  O **Elastic Load Balancing** distribui o tráfego entre as instâncias EC2 e envia métricas (como `CPUUtilization`) para o **Amazon CloudWatch**.
2.  Um **alarme do CloudWatch** monitora a métrica de utilização média da CPU do grupo.
3.  Quando a CPU média ultrapassa um limiar (ex: 60% por 5 minutos), o alarme do CloudWatch dispara e aciona uma política do **EC2 Auto Scaling**.
4.  O **Auto Scaling** usa a configuração de lançamento para adicionar uma nova instância EC2 ao grupo.
5.  O Auto Scaling então registra a nova instância no **ELB**.
6.  O **ELB** realiza verificações de saúde na nova instância e, quando ela estiver saudável, começa a enviar tráfego para ela.

### O que é o AWS Auto Scaling?
É um serviço separado que permite construir planos de escalonamento não apenas para instâncias EC2, mas também para outros recursos como frotas Spot, serviços ECS, tabelas DynamoDB e réplicas Aurora.

---

## Parte 5: Revisão Final e Questão Prática do Módulo

### Checklist de Aprendizagem do Módulo
* Distribuir tráfego entre instâncias EC2 usando o ELB.
* Identificar como o CloudWatch permite monitorar recursos em tempo real.
* Explicar como o EC2 Auto Scaling lança e encerra servidores em resposta a mudanças na carga de trabalho.
* Realizar tarefas de balanceamento para melhorar uma arquitetura.

### Análise de Questão Prática
* **A Pergunta:** "Qual serviço você usaria para enviar alertas com base em alarmes do Amazon CloudWatch?"
* **As Palavras-Chave:** "Enviar alertas" e "alarmes do Amazon CloudWatch".
* **A Resposta Correta e a Justificativa:** A resposta correta é **A, Amazon Simple Notification Service (SNS)**. Quando você cria um alarme no CloudWatch, você o configura para enviar uma notificação para um tópico do Amazon SNS. As outras opções são eliminadas porque, embora o CloudTrail possa enviar notificações para o SNS, a pergunta especifica que a base são os alarmes do CloudWatch, e o Trusted Advisor e o Route 53 têm outras finalidades.
