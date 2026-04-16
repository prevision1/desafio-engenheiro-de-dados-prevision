# Desafio Técnico - Engenharia de Dados

## Contexto

Somos um time de eficiência operacional responsável por desenvolver soluções que automatizam e melhoram processos internos da empresa. Um dos pilares do nosso trabalho é transformar dados dispersos em informação acionável para a tomada de decisão.

Atualmente, coletamos feedbacks de clientes a partir de múltiplas fontes (formulários, suporte, plataforma, e-mail, NPS) e já realizamos a centralização desses dados. O próximo passo é enriquecer esses feedbacks com métricas de negócio — como MRR, status de assinatura, plano e padrão de uso — para permitir análises mais estratégicas:

- Quais feedbacks vêm dos clientes de maior valor financeiro?
- Existe relação entre o tipo de feedback recebido e cancelamento?
- Qual tipo de plano tem mais fit com o produto (registra mais elogios)?

## Objetivo

Construir uma solução de dados que integre as fontes fornecidas, trate inconsistências, modele os dados de forma analítica e responda a perguntas de negócio concretas.

## Dados Fornecidos

Você receberá quatro arquivos que simulam dados reais do produto:

| **Arquivo**        | **Descrição**                                                  |
|--------------------|----------------------------------------------------------------|
| customers.csv      | Cadastro de clientes (plano, segmento, status, data de criação) |
| subscriptions.csv  | Histórico de assinaturas, com MRR e ciclo de cobrança          |
| feedbacks.csv      | Feedbacks coletados por diferentes canais                      |

> ⚠️ Os dados foram gerados para simular cenários reais. Espere encontrar inconsistências e lacunas — como IDs em formatos diferentes entre arquivos, registros duplicados, campos ausentes e clientes sem assinatura ativa. Parte do desafio é identificar e tratar esses problemas de forma explícita e justificada.

## O que Esperamos que Você Construa

A solução deve cobrir, no mínimo, estas três camadas:

### 1. Ingestão e Qualidade de Dados

- Leia e consolide os quatro arquivos
- Identifique e documente os problemas encontrados (duplicatas, nulos, inconsistências de formato, etc.)
- Aplique as tratativas que julgar adequadas, justificando cada decisão

### 2. Modelagem Analítica

- Modele os dados em uma estrutura que permita análise integrada
- A estrutura deve permitir cruzar feedbacks com métricas de negócio dos clientes

### 3. Análise Obrigatória

Sua solução deve ser capaz de responder, com evidências nos dados, à seguinte pergunta:

> *"Existe relação entre o tipo de feedback recebido e o churn de clientes? Como isso varia por segmento de plano?"*

Além dessa, sinta-se livre para explorar outras perguntas do contexto ou insights que surgirem ao longo da análise.

## Autonomia Técnica

Você tem total liberdade para definir:

- Stack e ferramentas (Python, SQL, dbt, Spark, DuckDB, Pandas, etc.)
- Onde os dados são armazenados (SQLite, DuckDB, arquivos Parquet, banco relacional, etc.)
- Como o pipeline é estruturado (scripts, notebooks, DAGs, etc.)
- Como a análise é apresentada (queries SQL, notebook, dashboard, gráficos, etc.)

Se houver informações ausentes ou ambíguas nos dados, assuma premissas — desde que estejam documentadas.

## Entregáveis

### Obrigatórios

- Repositório público (GitHub, GitLab ou similar) com código da solução
- README contendo:
  - Descrição da abordagem e arquitetura adotada
  - Decisões técnicas tomadas e seus trade-offs
  - Problemas de qualidade encontrados nos dados e tratamentos
  - Premissas assumidas
  - Instruções claras para execução local
  - Limitações da solução e possíveis evoluções

### Opcionais (valorizados)

- Diagrama da arquitetura ou do modelo de dados
- Testes automatizados
- Containerização (Docker)

## O que Vamos Avaliar

- Qualidade e organização do código
- Tratamento de qualidade de dados
- Modelagem de dados
- Capacidade analítica
- Documentação e comunicação técnica

> **Ênfase importante:** não buscamos solução perfeita. Preferência por solução menor e bem executada versus ampla e superficial. Clareza de raciocínio e capacidade de tomada de decisão pesam mais que volume de código.

## Tempo Estimado

Esperamos que o desafio seja realizado em 4 a 6 horas. Esse tempo é uma referência — não é necessário registrá-lo, mas ele sinaliza o nível de profundidade esperado.

## Apresentação

Após a entrega, você terá até 60 minutos para apresentar e debater a sua solução com o time técnico e de produto. Sugerimos cobrir:

- Breve explicação da arquitetura e das decisões tomadas
- Demonstração da análise obrigatória
- O que você faria diferente com mais tempo

Esteja preparado(a) para perguntas sobre suas escolhas técnicas e sobre os dados.

Qualquer dúvida sobre o desafio pode ser enviada para [email do recrutador]. Boa sorte!
