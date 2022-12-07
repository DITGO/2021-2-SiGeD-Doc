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

Os commits devem ser atômicos (uma contribuição pequena para resolver um problema específico), evite commitar muitas modificações de uma só vez. A mensagem do commit deve conter o que foi feito de maneira sucinta e direta, além disso ela precisa estar em inglês, começar com um verbo e com a primeira letra maiúscula. 

Exemplo de contribuição feita por um autor:
```
$ git commit -m "Adding quality control notebook"
```

Caso o commit tenha sido feito em cooperação com alguém, deve ser feita a co-autoria:

```
$ git commit -m "Create user model
>
>
Co-authored-by: name <name@example.com>
Co-authored-by: another-name <another-name@example.com>"
```

## Política de issues

Ao abrir uma issue obedeça o template para uma nova funcionalidade ou bug. 

```
### Nome da feature ou bug

#### Descrição
Pequena e objetiva descrição sobre a issue.

#### Objetivo
Descreva sucintamente o objetivo dessa issue

#### Tarefas
Seção para tarefas (tasks) para issues mais complexas ou sub-tarefas, como o exemplo abaixo.

- [ ] Adição de outro documento.
- [ ] Implementação do Cadastro.
- [ ] Redefinir senha.
- [ ] Alguma outra tarefa.

#### Contexto adicional
Alguma informação necessária para melhor compreensão, como o exemplo abaixo.

1. Após criar a issue, deve ser adicionado a pontuação da tarefa caso exista
2. Deve ser adicionado as labels pertinentes para a issue

#### Checklist
- [ ] A issue possui nome significativo.
- [ ] A issue possui descrição significativa.
- [ ] A issue possui screenshots quando necessárias.
- [ ] A issue possui labels.
```

## Política de Pull Request

<p style="text-align:justify">&emsp;&emsp;Para realizar um Pull Request (PR) para o repositório é necessário seguir os passos abaixo.
<ol>
<li> Comente na issue que deseja contribuir trazendo informações de como e quando irá finalizá-la;
<li> Ao resolver uma issue suba suas contribuições e crie um Pull Request na branch devel para ter seu Pull Request aceito;
<li> Escreva um título claro para identificação do Pull Request;
<li> O conteúdo do pull request deve ser constituído de uma lista contendo as principais modificações feitas, seguindo o template abaixo.

```
1. Descrição
2. Issue Relacionada
3. Como Isso Foi Testado?
4. Capturas de Tela (se apropriado):
5. Tipos de Mudanças
```

<li> Conecte o Pull Request com a issue que ele resolve;
<li> Preencha informações adicionais caso possua (executores, revisores, ...)
</ol>

<h3> Política aceitação de Pull Request </h3>

<p style="text-align:justify">&emsp;&emsp;Para realizar aceiter um Pull Request (PR) para o repositório é necessário cumprir os seguintes critérios de aceitação.

```
- [ ] Todos os críterios de aceitação atingidos;
- [ ] Cobertura de teste acima de 90 %;
- [ ] Etapas do CI passando;
- [ ] Ao menos 1 revisão de código com um revisor que não seja a mesma pessoa que realizou a issue;
- [ ] Seguir folha de estilo do projeto;
- [ ] Código em inglês;
```
