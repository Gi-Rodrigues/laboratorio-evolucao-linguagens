# Laboratório: Evolução das Linguagens de Programação

Projeto acadêmico para comparar implementações de um analisador de desempenho de turma em Python, C e JavaScript, além de observar os paradigmas procedural, funcional e orientado a objetos em Python.

## Estrutura

- `python/analisador.py`: valida notas e calcula as estatísticas da turma.
- `c/analisador.c`: implementação compilada em C.
- `javascript/analisador.js`: implementação executada com Node.js.
- `python/procedural.py`, `python/funcional.py` e `python/objetos.py`: exemplos de paradigmas.
- `testes/casos-testes.md`: entradas e resultados esperados.
- `docs/relatorio.md`: análise técnica da atividade.

## Executar

Na raiz do projeto, execute cada implementação com:

```bash
python3 python/analisador.py
node javascript/analisador.js
gcc c/analisador.c -o analisador && ./analisador
```

Para os exemplos de paradigmas:

```bash
python3 python/procedural.py
python3 python/funcional.py
python3 python/objetos.py
```

As três implementações principais usam a lista de exemplo `[8.5, 6.0, 9.0, 4.5, 7.0, 5.5, 3.0]`. Os resultados esperados estão documentados em `testes/casos-testes.md`.