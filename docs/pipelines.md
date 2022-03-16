<h1 style="text-align: center">Pipelines</h1>

<p style="text-align:justify">&emsp;&emsp;As pipelines de DevOps são scripts configurados em cada respositório do projeto que automatizam a execução de testes, verificações, coleta de métricas e deploy da aplicação. Para todos os microsserviços/repositórios do SiGeD para o semestre de 2021.2, os pipelines configurados seguem o seguinte padrão:</p>

## Testes

<p style="text-align:justify">&emsp;&emsp;O pipeline de testes é executado em qualquer ação git de <i>push</i> ou <i>pull request</i>. Esse pipeline é responsável por executar automaticamente os testes do microsserviço que sofreu alteração, informando no próprio repositório o sucesso ou não da execução dos testes.</p>

<p style="text-align:justify">&emsp;&emsp;Além disso, neste mesmo pipeline, caso a execução de testes tenha sucesso, o SonarCloud é acionado para a atualização do <i>Quality Gate</i>, disponibilizando várias métricas referentes a qualidade do código atual.</p>

## Lint

<p style="text-align:justify">&emsp;&emsp;O pipeline de lint é executado em qualquer ação git de <i>push</i> ou <i>pull request</i>. Esse pipeline é responsável por garantir que o código seja escrito de maneira manutenível. Através de uma série de regras, o script checa a existência de variáveis não utilizadas, espaços em excesso ou linhas muito longas, entre outros. Apesar de não afetar a execução do código, é de suma importância para manter o código legível e facilitar a entrada de novos desenvolvedores.</p>

## Extração de métricas

<p style="text-align:justify">&emsp;&emsp;O pipeline de extração de métricas é executado sempre que um <i>pull request</i> é merjado e fechado. O merge e fechamento de um <i>pull request</i> indica a finalização de uma task definida no backlog do produto. Sempre que tal ação é realizada, este pipeline gera um arquivo JSON na raíz do repositório com todas as métricas extraídas do SonarCloud. É importante para manter um histórico da situação de cada respositório e facilitar a visualização ao longo do tempo.</p>

## Deploy Contínuo

<p style="text-align:justify">&emsp;&emsp;O pipeline de deploy é executado quando há alguma ação git de <i>push</i> na branch master/main do repositório. Um <i>push</i> na master só pode ser realizado a partir da devel e após uma review completa do código novo a ser inserido. Na entrada de código novo na master, o pipeline de deploy derruba o microsserviço no servidor remoto, atualiza as informações remotas e sobe a aplicação novamente.</p>

<p style="text-align:justify">&emsp;&emsp;A execução deste pipeline deve ser observada com cuidado. Qualquer código que entrar na master sem ser revisado anteriormente pode gerar problemas no deploy, impossibilitando o acesso dos usuários à aplicação.</p>