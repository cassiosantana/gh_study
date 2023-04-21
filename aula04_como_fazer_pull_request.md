# Criando um pull request

Primeiramente devemos criar uma nova branch para fazer as alterações nela e seus commits para depois enviar para o github dando o push.

Se esta nova branch foi criada localmente, não pelo github, e for a primeira vez que for enviada receberemos um erro informando que ela não existe no github então teremos que rodar um comando que é sugerido pelo próprio git:

```sh
git push --set-upstream origin <nome da branch>
```

Como as alterações não foram feitas na main, o git pede para você fazer um pull request. Então lá github existirá uma notificação informando que foi realizado um push em uma branch que não é a main solicitando que seja realizado uma comparação e um possível pull request para realizar um merge.

Assim, um botão 'Compare & pull request' aparecerá.
Podemos notar que antes disso é possível trocar de branchs antes do pull request apenas para visualizar rapidamente.

Clicando no 'Compare & pull request' poderemos abrir um pull request, que nada mais é do que uma solicitação de merge, para que nosso código seja mesclado a main.
Devemos observar a branch de que queremos 'mergear' e qual irá receber o merge.

É importante também adicionar ao PR comentários informando o que foi realizado nesta branch para que a pessoa que irá analizar-lo entenda rápidamente e facilite sua análise.

Na lateral direita em 'Reviwers', devemos adicionar os usuários que irão analizar o PR no famoso Code Review. Quem irá analisar depende de cada empresa.

'Assignees' são as pessoas responsáveis pelo pela tarefa realizada na branch que estamos enviando para o PR.

'Labels' servem para que possamos colocar etiquetas referente ao que foi feito.

Abaixo do PR podemos visualizar os commits feitos na branch deste PR.

Para criar, depois de adicionar e revisar estes detalhes basta cliar em 'Create Pull Request'

Assim que criado ele terá seu número de identificação, lista de commits e quem foi responsável. o revisador pode solicitar algum comentário, etc... 

Depois de aprovado, é possível realizar o merge.

O fato de o PR já estar aberto não impede que façamos alterações. Caso o revisador perceba algum erro ele irá solicitar alterações no código, que podemos ver esta solicitação na página inicial do PR, que quando a efeturarmos podemos enviar o push para esta branch normalmente. A única diferença é que para dar este push é simplesmente 'git push' diferente do anterior que tem mais detalhes.

Após mergeado o status do PR muda e recebe a etiqueda roxa de 'Merged'.

O PR finalizado vai para a aba 'closed' para que possamos ter no histórico.
