# Entropia da fibra de um sistema aleatório

Seminário — *Cálculo numérico pelo método de Ulam* aplicado a um mapa aleatório do intervalo.
Autor: Edeilson Costa de Azevedo Filho.

## Estrutura

```
.
├── slides.tex              # apresentação (Beamer)
├── slides.pdf              # apresentação compilada
├── figuras.ipynb           # notebook que gera todas as figuras
└── figs/                   # figuras usadas nos slides (geradas pelo notebook)
```

## Como reproduzir

1. Gerar as figuras (salvas em `figs/`):
   ```bash
   jupyter nbconvert --to notebook --execute figuras.ipynb
   ```
   Dependências: `numpy`, `matplotlib`.

2. Compilar os slides:
   ```bash
   latexmk -pdf slides.tex
   ```
