# Entropia da fibra de um sistema aleatório

Seminário — *Cálculo numérico pelo método de Ulam* aplicado ao mapa aleatório de Pelikan.
Autor: Edeilson Costa de Azevedo Filho.

## Estrutura

```
.
├── slides.tex              # apresentação (Beamer)
├── slides.pdf              # apresentação compilada
├── pelikan_figuras.ipynb   # notebook que gera todas as figuras
└── figs/                   # figuras usadas nos slides (geradas pelo notebook)
```

## Como reproduzir

1. Gerar as figuras (salvas em `figs/`):
   ```bash
   jupyter nbconvert --to notebook --execute pelikan_figuras.ipynb
   ```
   Dependências: `numpy`, `matplotlib`.

2. Compilar os slides:
   ```bash
   latexmk -pdf slides.tex
   ```
