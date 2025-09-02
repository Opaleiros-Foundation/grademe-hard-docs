# Ranking

## Pontos importantes de como será feito o ranking

### Calculo Overral

**Fórmula “Game-like” (não linear)**

Às vezes jogos dão peso maior para atributos altos, aplicando exponenciação:

$$
Overall = \frac{\sum (x_i^{\alpha} \cdot w_i)}{\sum w_i}
$$

* Se **α > 1** → atributos altos têm mais impacto.
* Se **0 < α < 1** → atributos baixos têm mais impacto.
