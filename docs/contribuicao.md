<h1 style='text-align: center;'>Políticas de Contribuição</h1>

## Como contribuir?

* Primeiro, certifique-se de navegar pelos repositórios e ler a documentação para se familiarizar com o projeto.
* Escolha uma task para inciar o desenvolvimento ou, caso identifique um problema no software, crie uma task nova.
* Crie uma branch a partir da devel conforme descrito abaixo.
* No caso de usuários externos, utilize um fork do projeto.
* Ao finalizar a implementação, inicie um Pull Request e aguarda a revisão.

## Políticas de branches

**main/master**

<p style="text-align:justify">&emsp;&emsp;A branch main/master é a branch principal do projeto, onde se encontra o código que está em produção, disponível para os usuários. Essa branch não deve ser modificada sem supervisão dos administradores do projeto.</p>

**devel**

<p style="text-align:justify">&emsp;&emsp;A branch devel é a branch a partir de qual todas as outras devem ser criadas. Qualquer nova funcionalidade implementada/bug corrigido será primeiro inserido na devel, testado e somente após uma revisão completa será admitido na main/master.</p>

**Novas branches**

<p style="text-align:justify">&emsp;&emsp;Ao criar novas branches a partir da devel, siga o seguinte formato para a nomenclatura da branch:</p>

* Branch de correção de bug/defeito: **fix**/descrição-do-bug
* Branch de implementação de nova funcionalidade: **feature**/descrição-da-feature
* Branch de implementação de melhoria em uma funcionalidade já existente: **improvement**/descrição-da-melhoria

## Política de commits

<p style="text-align:justify">&emsp;&emsp;As mensagens de commit devem ser escritas em inglês e detalharem o que foi realizado de forma resumida. Evite commitar muitas modificações de uma só vez.</p>

## Abertura de issues

<p style="text-align:justify">&emsp;&emsp;Ao abrir uma nova issue, escolha um dos templates fornecidos, a depender do que a issue irá apresentar. Respeite o template para facilitar a identificação de Histórias de Usuários e tasks.</p>