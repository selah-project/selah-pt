# Como contribuir para a versão portuguesa de Selah

Obrigado por ajudar a tornar esta versão mais exata, clara e natural. Não é
preciso ser especialista para apontar um problema: diga o que observou,
apresente sua evidência e diferencie certeza de sugestão.

## Questão ou pull request

- Abra uma **issue** quando a leitura precisar de discussão, houver mais de uma
  opção possível ou você não souber como alterar o registro alinhado.
- Abra um **pull request** quando o erro e a substituição exata estiverem claros.
- Para erros do aplicativo ou assuntos privados de segurança, conta ou dados
  pessoais, use [o suporte de Selah](https://selahproject.com/support).

## O que incluir

Informe livro, capítulo, versículo e token hebraico; texto atual; texto
proposto; razão da mudança; e fonte lexical, gramatical, contextual ou publicada.
Diga se o português é sua língua materna e se você lê o hebraico diretamente.

## Como editar um registro

Os arquivos ficam em `<livro>/<capítulo>/<versículo>.json`.

- Altere `translation` e o `gloss` do token correspondente quando ambos forem
  afetados.
- Preserve `book`, `chapter`, `verse`, `ref`, os valores hebraicos `surface`, a
  ordem e a quantidade de tokens, salvo em uma correção de alinhamento.
- Não altere modelo, nível, data ou procedência apenas para fazer a correção
  parecer uma nova geração.
- Preserve as convenções de colchetes, Nomes divinos e `⟨את⟩`.
- Evite mudanças apenas de formatação e correções não relacionadas.

Valide o JSON editado:

```bash
python3 -m json.tool genesis/1/1.json >/dev/null
```

O hebraico vem primeiro. Quando duas leituras forem defensáveis, explique a
diferença em vez de apresentar preferência como certeza. Não copie uma
tradução moderna protegida por direitos autorais.

## Trabalho assistido por IA

Declare o uso relevante de modelos de linguagem ou tradução automática e a
revisão humana realizada. Não envie reescritas em massa sem revisão. A pessoa
que contribui continua responsável por cada palavra proposta.

## Licença, atribuição e revisão

Ao contribuir, você declara ter o direito de fazê-lo e concorda que o material
aceito seja distribuído sob [CC BY-SA 4.0](LICENSE.md). O histórico do Git
preserva o registro público e a atribuição. A manutenção compara a proposta com
o hebraico, as convenções, as fontes e o alinhamento. Ela pode aceitar, revisar
com você, aguardar mais evidências ou recusar explicando a razão. Critique a
leitura, não a pessoa.

## Conduct

Be honest, be kind, show your evidence. Distinguish certainty from
suggestion. The maintainers weigh and decide.
