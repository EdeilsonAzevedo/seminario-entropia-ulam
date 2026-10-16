# Entropia da fibra de um sistema aleatório

Seminário — *Cálculo numérico pelo método de Ulam* aplicado a um mapa aleatório do intervalo.
Autor: Edeilson Costa de Azevedo Filho.

## Estrutura

```
.
├── slides.tex              # apresentação (Beamer)
├── slides.pdf              # apresentação compilada
├── figuras.ipynb           # notebook que gera todas as figuras
├── figs/                   # figuras usadas nos slides (geradas pelo notebook)
└── apostila/               # seção da apostila sobre o mapa de Pelikan
    ├── secao_pelikan.tex   # texto da seção (usar com \input{secao_pelikan})
    ├── preview_apostila.tex# documento mínimo para pré-visualizar a seção
    └── figs/               # figuras usadas na seção
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

3. Pré-visualizar a seção da apostila:
   ```bash
   cd apostila && latexmk -pdf preview_apostila.tex
   ```
