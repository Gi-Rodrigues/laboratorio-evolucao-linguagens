# Relatório técnico

## 1. Linguagem que exigiu mais código

C exigiu mais declarações explícitas: é necessário definir os tipos das variáveis, percorrer o vetor, acumular a soma e atualizar os contadores. Python e JavaScript oferecem operações de coleção que deixam algumas etapas mais concisas.

## 2. Declaração e uso das variáveis

Em C, variáveis e elementos do vetor têm tipos declarados, como `float` e `int`. Em Python e JavaScript, o tipo é associado ao valor em execução. No JavaScript, `const` impede a reatribuição da variável, mas não torna imutável o conteúdo de um objeto ou array.

## 3. Compilação explícita

Neste experimento, C exige compilação explícita com `gcc c/analisador.c -o analisador` antes de executar `./analisador`. Python é executado pelo interpretador e JavaScript pelo Node.js; não há uma etapa de compilação manual nos comandos da atividade.

## 4. Tipagem e validação

Python verifica o tipo com `isinstance` e rejeita booleanos, embora `bool` seja uma subclasse de `int`. JavaScript verifica o tipo, a finitude e os limites com `typeof` e `Number.isFinite`. C recebe valores `float` no vetor, então a validação verifica se estão entre 0 e 10.

## 5. Simplicidade e manutenção

Para este problema pequeno, Python é direto de ler por causa de funções como `sum`, `max` e `min`. JavaScript também é conciso ao usar `reduce` e `filter`. C deixa o processamento mais explícito, o que pode ser útil quando se deseja controlar tipos e operações em baixo nível.

## 6. Riscos de aceitar dados sem validação

Uma nota fora do intervalo ou de tipo inesperado poderia distorcer a média e as contagens, gerando uma classificação incorreta. Em C, acessar uma coleção vazia para inicializar maior e menor também seria inválido; por isso o tamanho deve ser verificado antes do acesso.

## 7. Contribuição do Git

O Git permite acompanhar as alterações em cada implementação, consultar versões anteriores e registrar a evolução por commits. O histórico também ajuda a identificar quando uma mudança foi feita e por quem.

## 8. `git add`, `git commit` e `git push`

`git add` seleciona as alterações para o próximo registro; `git commit` cria esse registro no histórico local; `git push` envia commits locais para o repositório remoto.

## 9. Salvar no Codespaces e enviar ao GitHub

Salvar grava o conteúdo do arquivo no ambiente de trabalho. Isso não cria um commit nem envia a mudança ao GitHub. Para publicar, é necessário adicionar e commitar as alterações e depois executar `git push`.

## 10. Escolha de linguagem

Python é adequado para scripts, análise de dados e prototipagem rápida. C é uma opção quando controle de recursos e integração de baixo nível são importantes. JavaScript é apropriado para aplicações web e serviços que utilizam o ecossistema Node.js. A escolha depende dos requisitos e do ambiente do sistema.

## Resultados da execução

Com a lista de exemplo, as três implementações devem apresentar 7 estudantes, média 6,21, maior nota 9,00, menor nota 3,00, 3 aprovados, 2 em recuperação e 2 reprovados. Os comandos de execução estão no README.
