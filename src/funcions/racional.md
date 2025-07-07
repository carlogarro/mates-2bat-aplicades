# Funció racional

Una **funció racional** és el quocient de dues funcions polinòmiques, és a dir, una funció de la forma:

\\[
f(x) = \frac{P(x)}{Q(x)}
\\]

on \\(P(x)\\) i \\(Q(x)\\) són polinomis, i \\(Q(x) \neq 0\\).

## Domini

El domini d'una funció racional són tots els valors reals per als quals el denominador Q(x) no és zero, ja que dividir per zero no està definit.

\\[
\operatorname{dom}(f) = \{ x \in \mathbb{R} \mid Q(x) \neq 0 \}
\\]

## Exemples

\\[
f(x) = \frac{x^2 - 1}{x - 3}
\\]

el domini és \\(\mathbb{R} \setminus \\{3\\}\\), és a dir, tots els reals menys \\(x=3\\).

<div id="jxgbox" class="jxgbox" style="width:500px; height:300px; margin: 0 auto;"></div>
<script>
  const board = JXG.JSXGraph.initBoard('jxgbox', {
    boundingbox: [-15, 20, 20, -15],
    axis: true,
    showCopyright: false,
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

---

\\[
f(x) = \frac{1}{x - 3}
\\]

La funció no està definida quan el denominador s’anul·la:
\\( x - 3 = 0 \Rightarrow x = 3 \\)

Per tant,

\\[
\operatorname{dom}(f) = \mathbb{R} \setminus \{3\}
\\]

<div id="jxgbox1" class="jxgbox" style="width:400px; height:300px; margin: 0 auto;"></div>
<script>
  const b1 = JXG.JSXGraph.initBoard('jxgbox1', {
    boundingbox: [-5, 5, 10, -5],
    axis: true,
    showNavigation: true,
    showCopyright: false
  });
b1.create('functiongraph', [
function(x) {
return 1 / (x - 3);
}, -5, 10
], {
strokeColor: 'blue',
dash: 0
});
b1.create('line', [[3, -10], [3, 10]], {
strokeColor: 'red',
dash: 2,
straightFirst: false,
straightLast: false
});
</script>

---

\\[
f(x) = \frac{x + 1}{x^2 - 4}
\\]

Denominador: \\( x^2 - 4 = 0 \Rightarrow x = \pm 2 \\)

Per tant,

\\[
\operatorname{dom}(f) = \mathbb{R} \setminus \\{-2, 2\\}
\\]

<div id="jxgbox2" class="jxgbox" style="width:400px; height:300px; margin: 0 auto;"></div>
<script>
  const b2 = JXG.JSXGraph.initBoard('jxgbox2', {
    boundingbox: [-5, 5, 5, -5],
    axis: true,
    showNavigation: true,
    showCopyright: false
  });
b2.create('functiongraph', [
function(x) {
return (x + 1) / (x*x - 4);
}, -5, 5
], {
strokeColor: 'blue'
});
b2.create('line', [[-2, -10], [-2, 10]], {
strokeColor: 'red',
dash: 2,
straightFirst: false,
straightLast: false
});
b2.create('line', [[2, -10], [2, 10]], {
strokeColor: 'red',
dash: 2,
straightFirst: false,
straightLast: false
});
</script>
