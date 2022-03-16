
# Introdução 

A função do Plano de Gerenciamento de Riscos é definir como serão conduzidas as atividades de gestão de risco, ou seja, informar quais serão as medidas adotadas para lidar com as possíveis ameaças ou oportunidades.

Conforme o PMBOK, existem sete processos que são essenciais para um bom gerenciamento de riscos. São eles:

- Planejar o gerenciamento dos riscos;
- Identificar os riscos;
- Realizar a análise qualitativa dos riscos;
- Realizar a análise quantitativa dos riscos;
- Planejar as respostas aos riscos;
- Implementar respostas aos riscos;
- Monitorar os riscos.  

- - -

## Glossário

| Termo	| Significado | 
| -------- | -------- | 
|RN | Risco Negativo|  
|RP | Risco Positivo|
- - -

## Identificação de riscos

A identificação de riscos se refere ao mapeamento dos riscos individuais e gerais do projeto e suas características. O principal benefício desse é trazer informações para que a equipe consiga responder de forma adequada a esses riscos, independentemente se eles forem ameaças ou oportunidades.  

- Os riscos com efeito negativo são as ameaças ao projeto.
- Os riscos com efeito positivo são as oportunidades do projeto.

Os riscos serão identificados durante os eventos Scrum, reuniões de planejamento e pareamentos.  


### Riscos Negativos

| Causa	| Risco	| Descrição do risco	| Impacto |
| -------- | -------- | -------- | -------- |
| Inexperiência do time | RN1 | Dificuldades com as tecnologias utilizadas | Baixa produtividade, atraso nas entregas e sobrecarga de membros. |
| Problemas de conexão | RN2 | Problemas com a internet, energia e afins | Atraso nas entregas ou sobrecarga de outros membros |
| Problemas de hardware | RN3 | Problemas no hardware para rodar os ambientes | Atraso nas entregas ou sobrecarga de outros membros |
| Escopo mal definido | RN4 | Visão geral do produto mal definida | Retrabalho |
| Problemas pessoais | RN5| Problemas pessoais dos membros da equipe  | Mudança no Planejamento, atrasos, sobrecarga. |
| Divergência de horários entre os membros | RN6 | Membro do time não conseguir participar das reuniões com os P.O's ou reuniões do time | Falta de entendimento do membro do time acerca da situação do projeto |
| Desistência de membros da equipe | RN7 | Membro do time desistir do projeto durante o desenvolvimento | Atraso nas entregas, sobrecarga de outros membros e impacto no escopo do projeto |
| Baixa qualidade do produto | RN8 | Pruduto com defeitos de desenvolvimento  | Não atender às expectavivas do cliente  |


### Riscos Positivos
| Causa	| Risco	| Descrição	| Impacto |
| -------- | -------- | -------- | -------- |
| Motivação com o projeto | RP1 | Interesse da equipe em evoluir e continuar no projeto | Continuidade do projeto e aumento de produtividade|
| Produtividade | RP2 | Entregas de acordo com o previsto | Segurança para o cliente de que suas expectativas serão atendidas |
| Entregas antes do prazo | RP3 | Entregas antes do cronograma estabelecido | Aumento na qualidade do projeto e possível aumento do escopo |


## Análise Qualitativa de Riscos
A análise qualitativa dos riscos consiste em priorizar os riscos individuais identificados, considerando principalmente sua probabilidade de ocorrência e seus impactos nos objetivos do projeto.  
A probabilidade será categorizada conforme a tabela abaixo.

### Probabilidade 

| Probabilidade (P)	 | Intervalo de ocorrência | Peso |
| -------- | -------- | -------- |
| Muito Baixa | 0 <= P <=20% | 1 |
| Baixa | 20% < P <= 40%| 2 |
| Moderada | 40% < P <= 60% | 3 |
| Alta | 60% < P <= 80% | 4 |
| Muita Alta | 80% < P <= 100% | 5 |

### Impacto
O impacto varia de acordo como os riscos afetam o projeto.

| Impacto - (I) | Descrição | Peso |
| -------- | -------- | -------- |
| Muito Baixa | Quase  imperceptível ao projeto.| 1 |
| Baixa | Pouca influência no projeto. | 2 |
| Moderada | Notável ao projeto, mas com poucas consequências. | 3 |
| Alta | Dificulta a realização projeto. | 4 |
| Muita Alta | Impossibilita a realização do projeto. | 5 |


### Riscos Negativos

| Risco | Probabilidade | Impacto |	Prioridade |
| -------- | -------- | -------- | -------- |
| RN1 | Muito alta | Alto | Alta |
| RN2 | Moderada | Muito Baixa | Baixa |
| RN3 | Moderada | Muito Baixa | Baixa |
| RN4 | Moderada | Muito Alto | Muito Alta |
| RN5 | Alta | Moderada | Moderada | 
| RN6 | Muito Alta | Moderada | Moderada | 
| RN7 | Baixa | Moderada | Moderada | 
| RN8 | Moderada | Muito Alta | Alta | 

### Riscos Positivos

| Risco | Probabilidade | Impacto |	Prioridade |
| -------- | -------- | -------- | -------- |
| RP1 | Moderada | Alto | Alta |
| RP2 | Baixa | Alto | Moderada |
| RP3 | Baixa | Moderada | Baixa |

## Planejando Respostas aos Riscos
Esta estapa consiste em desenvolver alternativas, selecionar estratégias e acordar ações para lidar com a exposição geral aos riscos e tratar os riscos individuais. 

|  Risco| Estratégia | Resposta |
| -------- | -------- | -------- |
| RN1 | Prevenir | Indentificar o nível de conhecimento do time e fazer os treinamentos necessários   |
| RN2 | Consertar falhas | Transferir a tarefa para outro membro do time ou adaptação para sua execução |
| RN3 | Consertar falhas | Possuir alternativas para quando há problemas no hardware de algum dos membros |
| RN4 | Prevenir | Durante os encontros do time, identificar eventuais no escopo o quanto antes|
| RN5 | Gerenciar | É um risco em que as ações de prevenção não são cabíveis à equipe, mas é possível fazer o gerenciamento conformer andamento do projeto |
| RN6 | Mitigar | Tentar encaixar horários com o maior número de membros da equipe disponível |
| RN7 | Consertar falhas | Não há muito como prever mas, ao acontecer, realocar tarefas entre os membros da equipe, evitando sobrecarregá-los |
| RN8 | Prevenir | Utilizar ferramentas de testes automatizados para verificar a qualidade do código |
| RP1 | Aceitar | Incentiva os membros da equipe continuamente para que continuem motivados |
| RP2 | Aceitar | Acompanhar métricas de produtividade da equipe e tomar ações no decorrer do planejamento das sprints |
| RP3 | Aceitar | Propor aumento de escopo, respeitando prazos e limitações da equipe |

## Implementando respostas de risco

A equipe estará monitorando os riscos apresentados durante os eventos SCRUM. Se caso algum deles ou outro inesperado ocorra, será implementada a resposta ao risco.

## Monitoramento de Riscos


| Risco | Monitoramento 
| -------- | -------- |
| R1 | Através do pareamento e das reuniões diárias |
| R2 | Através das reuniões diárias e canais de comunicação da equipe  |
| R4 | Atráves das reuniões com os clientes e pelo roadmap |
| RN4 | Através das reuniões diárias e canais de comunicação da equipe |
| RN5 | Através dos canais de comunicação da equipe |
| RN6 | Através das reuniões diárias e canais de comunicação da equipe |
| RN7 | Atráves do sonarcloud e dos testes automatizados |
| RP1 | Através das reuniões diárias e canais de comunicação da equipe |
| RP2 | Através da metodologia ágil, terá acompanhamento constante da produtividade da equipe |
| RP3 | Através do cronograma do projeto |

- - -

## Referências

EUAX. Gerenciamento de Riscos em Projetos: aprenda a lidar com as incertezas na gestão de iniciativas. Disponível em: https://www.euax.com.br/2018/02/importancia-do-gerenciamento-de-riscos/. Acesso em: 15 mar. 2022.


## Histórico

| Versão | Data       | Modificação                    | Autor(es) |
| ------ | ---------- | ------------------------------ | ----- |
| 0.1    | 14/03/2022 | Criação do documento  | Nícalo |
| 0.2    | 15/03/2022 | Desenvolvimento do documento | Nícalo, Murilo, Gabriel e Rafael |
| 1.0    | 15/03/2022 | Finalização da primeira versão e revisão | Nícalo, Murilo, Gabriel e Rafael |
