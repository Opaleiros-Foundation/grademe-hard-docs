# Ranking

## Pontos importantes de como será feito o ranking

### Calculo Overral

## 1. **Média Ponderada (clássica)**

Cada atributo tem um peso (`w`) e um valor (`x`).

$$
Overall = \frac{\sum (x_i \cdot w_i)}{\sum w_i}
$$

Exemplo:

* Força = 80 (peso 0.4)
* Velocidade = 70 (peso 0.3)
* Inteligência = 90 (peso 0.3)

$$
Overall = \frac{80 \cdot 0.4 + 70 \cdot 0.3 + 90 \cdot 0.3}{0.4 + 0.3 + 0.3} = 81
$$

---

## 2. **Média Aritmética Simples (se pesos forem iguais)**

$$
Overall = \frac{\sum x_i}{n}
$$

Bom quando todos os atributos têm a mesma importância.

---

##  3. **Média Geométrica (mais rigorosa)**

$$
Overall = \left(\prod x_i^{w_i}\right)^{\frac{1}{\sum w_i}}
$$

Castiga bastante quem tem atributos baixos.
Se um atributo for **muito fraco**, o overall cai forte.

---

## 4. **Média Harmônica (ênfase nos menores valores)**

$$
Overall = \frac{\sum w_i}{\sum \frac{w_i}{x_i}}
$$

Excelente quando você quer que o **pior atributo pese mais** (ex.: times em que a fraqueza não pode ser escondida).

---

## 5. **Weighted Percentile / Normalização**

Se os atributos estiverem em escalas diferentes, normalize antes (0–1 ou 0–100).
Exemplo (min-max normalization):

$$
x'_i = \frac{x_i - min(x)}{max(x) - min(x)}
$$

Depois aplique a **média ponderada** sobre os valores normalizados.

---

## 6. **Fórmula “Game-like” (não linear)**

Às vezes jogos dão peso maior para atributos altos, aplicando exponenciação:

$$
Overall = \frac{\sum (x_i^{\alpha} \cdot w_i)}{\sum w_i}
$$

* Se **α > 1** → atributos altos têm mais impacto.
* Se **0 < α < 1** → atributos baixos têm mais impacto.

---

Resumindo:

* **Justo / equilibrado → Média ponderada.**
* **Quer punir fraquezas → Harmônica / Geométrica.**
* **Quer destacar atributos fortes → Exponencial.**

