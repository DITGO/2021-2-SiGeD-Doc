<h1 style="text-align: center">Planejamento de Custo</h1>

<p style="text-align:justify">&emsp;&emsp;Para gerar um estimativa de custo, foi levado em consideração todos os aspectos do projeto que geram gastos direta ou indiretamente. São esses gastos: custo de pessoal, custo de equipamento, custo de infraestrutura e custos adicionais (energia elétrica e internet).</p>

<p style="text-align:justify">&emsp;&emsp;Para a estimativa, foi considerado um total de 9 sprints semanais, começando no dia 26 de fevereiro e terminando no dia 30 de abril.</p>

<iframe width="100%" height="480px" style={{minWidth: "640px", minHeight: "480px", backgroundColor: "#f4f4f4", border: "1px solid #efefef" }} src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQNj9JtHHKWZlqpceKlAqxQx3Yd5zYE1czHST0eZfmOZPkOHaj5pRt_nskqU5PW1MuizHGORWR_3FL7/pubhtml"></iframe>

<a href="https://docs.google.com/spreadsheets/d/1_ZsynnNEx508iuZfXJVnvge0Pf39QJewoOO-s2Le-5Q/edit?usp=sharing">Visualização da Planilha</a>

## Custo de pessoal

<p style="text-align:justify">&emsp;&emsp;O projeto será desenvolvido no decorrer de 9 sprints com 10 horas semanais dedicadas por cada estudante. Levando em consideração que o custo médio anual de um estudante em universidades federais do Brasil é de R$38.805,00 (retirado de <a href="https://infograficos.oglobo.globo.com/brasil/raio-x-do-custo-por-aluno-nas-universidades-federais.html">O Globo - Raio-X do custo...</a>), o cálculo do custo/hora de cada desenvolvedor do projeto é o seguinte:</p>

>```Custo anual por estudante/365/24``` = ```R$ 4,43 / hora```

## Custo de equipamento

<p style="text-align:justify">&emsp;&emsp;O custo de equipamento diz respeito as máquinas que serão utilizadas pelos desenvolvedores durante o período de desenvolvimento do projeto. Levando em consideração que o projeto é dividido em 6 microsserviçoes que devem rodar simultaneamente para a execução dos testes necessários, as especificações da máquina devem ser adequadas para tal. Levando isso em consideração, o sistema escolhido para o desenvolvimento possui as seguintes especificações: 8GB de RAM, processaor Intel Core i7 e um SSD de 256GB (menor tamanho disponível).</p>

<p style="text-align:justify">&emsp;&emsp;O valor de cada máquina foi obtido através de um <a href="https://www.zoom.com.br/notebook/processador-intel-core-i7/memoria-8-gb/com-ssd/ssd-256gb?gclid=CjwKCAiAprGRBhBgEiwANJEY7MAyC31o06LebTeoZr92ZIhMxZZjt9IvXxfKhQJDJGORoRvrxRn6iRoCiCkQAvD_BwE&og%5B0%5D=18000&og%5B1%5D=18000&pageTitle=Notebook+Intel+Core+i7+8+GB+Sim&q=&sortBy=price_asc">site comparador de preços</a>. Dessa forma, o cálculo do custo de equipamento é dado por:</p>

>```Quantidade de membros do time``` X ```Preço unitário da máquina especificada``` = ```Custo total com equipamento```

## Custo de infraestrutura

<p style="text-align:justify">&emsp;&emsp;O custo de infraestrutura diz respeito a hospedagem do projeto em um servidor remoto, para que os usuários tenham acesso ao produto durante o desenvolvimento. Como o SiGeD será de uso interno da DPSS, o projeto não será disponibilizado em lojas de aplicativo, como PlayStore e AppStore.</p>

<p style="text-align:justify">&emsp;&emsp;Atualmente, o projeto está sendo hospedado em uma máquina da DigitalOcean. A máquina possui 8GB RAM, uma CPU Intel de 4 núcleos e 50 gigabytes de SSD, com um custo de 20,00 dólares ao mês. Como a máquina será de uso exclusivo do SiGeD, a capacidade atual é aceitável para o desempenho adequado do sistema.</p>

<p style="text-align:justify">&emsp;&emsp;Dessa forma, o cálculo da infraestrutura é dado por:</p>

>```Quantidade de meses de hospedagem``` X ```Valor da hospedagem``` = ```Custo total com infraestrutura```

## Custos adicionais

<p style="text-align:justify">&emsp;&emsp;Os custos adicionais dizem respeito a gastos indiretos decorrentes do desenvolvimento do projeto. No caso do desenvolvimento remoto, como será esse semestre, os gastos adicionais se resumem primariamente a energia elétrica e internet durante o uso dos equipamentos.</p>

<p style="text-align:justify"><b>Energia elétrica:</b> para o cálculo da energia elétrica, o grupo realizou uma <a href="https://g1.globo.com/df/distrito-federal/noticia/2020/12/01/conta-de-luz-fica-mais-cara-no-df-apos-reajuste-da-aneel.ghtml">pesquisa</a> do consumo médio mensal de energia no DF, gerando uma <a href="https://g1.globo.com/df/distrito-federal/noticia/2021/10/22/conta-de-luz-fica-mais-cara-no-df-a-partir-desta-sexta-feira-22.ghtml">pesquisa</a> da tarifa que esse consumo resulta. Levando em consideração que a máquina escolhida consome em torno de 0,065Wh, de acordo com as especificações, o cálculo do custo de energia elétrica diário é dado por:</p>

>```Tarifa média no DF``` X ```Consumo por hora do aparelho``` X ```Quantidade de horas trabalhadas``` X ```Quantidade de desenvolvedores``` = ```Custo total com energia elétrica diário```

<p style="text-align:justify"><b>Internet:</b> para o cálculo da internet, o grupo realizou uma pesquisa em <a href="https://melhorplano.net/internet-banda-larga/df/brasilia">site comparativo</a> sobre os planos de internet disponíveis no DF. Para a execução do projeto, o grupo levantou que um plano de 250Mb é ideal. Dessa forma, o cálculo do custo de internet mensal é dado por:</p>

>```Custo do plano contratado``` X ```Quantidade de desenvolvedores``` = ```Custo total com internet```

## Histórico

| Versão | Data       | Modificação                    | Autor(es) |
| ------ | ---------- | ------------------------------ | ----- |
| 0.1    | 14/03/2022 | Criação do documento  | Murilo |
| 0.2    | 15/03/2022 | Desenvolvimento do documento | Murilo |
| 1.0    | 15/03/2022 | Finalização da primeira versão e revisão | Nícalo, Murilo e Rafael |