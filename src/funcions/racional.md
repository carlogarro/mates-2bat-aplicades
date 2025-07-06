# Funció racional

Una **funció racional** és el quocient de dues funcions polinòmiques, és a dir, una funció de la forma:

\\[
f(x) = \frac{P(x)}{Q(x)}
\\]

on \\(P(x)\\) i \\(Q(x)\\) són polinomis, i \\(Q(x) \neq 0\\).

---

## Domini

El domini d’una funció racional és l’ensemble de tots els valors reals \(x\) per als quals el denominador no és zero:

\\[
\mathrm{Dom}(f) = \{ x \in \mathbb{R} \mid Q(x) \neq 0 \}
\\]

Per exemple, per la funció

\\[
f(x) = \frac{x^2 - 1}{x - 3}
\\]

el domini és \(\mathbb{R} \setminus \{3\}\), és a dir, tots els reals menys \(x=3\).

---

## Exemple amb gràfic

A continuació veiem la gràfica de la funció racional

\\[
f(x) = \frac{x^2 - 1}{x - 3}
\\]

amb un clar forat vertical a \(x=3\).

<div id="jxgbox" class="jxgbox" style="width:500px; height:300px;"></div>
<script>
  const board = JXG.JSXGraph.initBoard('jxgbox', {
    boundingbox: [-15, 20, 20, -15],
    axis: true,
    pan: {
      enabled: true,  // permet moure el gràfic amb el ratolí
      needShift: false // no cal prémer Shift per moure (opcional)
    },
    zoom: {
      enabled: true,  // permet fer zoom amb roda del ratolí
      wheel: true,
      needShift: false
    }
  });
  const f = function(x) {
    return (x*x - 1) / (x - 3);
  };
  board.create('functiongraph', f, {strokeColor:'#00a', strokeWidth:2});
  board.create('line', [[3, -5], [3, 5]], {
    strokeColor: 'red', dash: 2, strokeWidth: 1, fixed: true
  });
</script>
