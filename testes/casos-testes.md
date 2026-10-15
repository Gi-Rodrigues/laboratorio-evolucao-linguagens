# Casos de teste

## Resultado da lista de exemplo

Entrada: `[8.5, 6.0, 9.0, 4.5, 7.0, 5.5, 3.0]`

Resultado esperado nas três linguagens:

| Indicador | Esperado |
| --- | ---: |
| Quantidade | 7 |
| Média | 6,21 |
| Maior nota | 9,00 |
| Menor nota | 3,00 |
| Aprovados (nota >= 7) | 3 |
| Recuperação (5 <= nota < 7) | 2 |
| Reprovados (nota < 5) | 2 |

## Validação de entradas

Para testar estes casos, substitua temporariamente a lista fixa no código da linguagem correspondente e execute novamente.

| Entrada | Resultado esperado |
| --- | --- |
| `[0, 5, 7, 10]` | Válida; média 5,50; 2 aprovados, 1 em recuperação e 1 reprovado. |
| `[]` | Rejeitada como lista vazia por Python e JavaScript. Em C, o vetor fixo deve ser alterado para uma solução de entrada dinâmica para representar uma lista vazia. |
| `[-1, 6, 11]` | Rejeitada por conter nota fora do intervalo de 0 a 10. |
| `[6, "sete"]` em Python | Rejeitada por conter valor que não é numérico. |
| `[6, True]` em Python | Rejeitada; booleanos não são aceitos como notas. |
| `[6, NaN]` em JavaScript | Rejeitada por `Number.isFinite`. |

## Execução

Na raiz do repositório:

```bash
python3 python/analisador.py
node javascript/analisador.js
gcc c/analisador.c -o analisador && ./analisador
```

Os valores inválidos devem interromper o processamento e apresentar a mensagem de erro definida na implementação. Depois de testar entradas modificadas, restaure a lista de exemplo antes de comparar os resultados padrão.
