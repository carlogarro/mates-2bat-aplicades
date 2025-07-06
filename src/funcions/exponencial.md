# Funció exponencial

Una **funció exponencial** és de la forma:

\\[
f(x) = a^x
\\]

on la base \\(a\\) és un nombre real positiu diferent de \\(1\\) (\\(a > 0, a \neq 1\\)).

---

## Domini

El domini de la funció exponencial és tot \(\mathbb{R}\):

\\[
\mathrm{Dom}(f) = \mathbb{R}
\\]

La funció està definida per a qualsevol nombre real \(x\).

---

## Exemple amb gràfic

Considerem la funció exponencial amb base 2:

\\[
f(x) = 2^x
\\]

<div id="jxgbox" class="jxgbox" style="width:500px; height:300px;"></div>
<script>
  var board = JXG.JSXGraph.initBoard('jxgbox', {
  boundingbox: [-2, 10, 4, -10],
  axis: true,
  pan: { enabled: true, needTwoFingers: false, needShift: false },
  zoom: { enabled: true, factorX: 1.25, factorY: 1.25, wheel: true, needShift: false },
  showCopyright: false
});
  const f = function(x) {
    return Math.pow(2, x);
  };
  board.create('functiongraph', f, {strokeColor:'#d22', strokeWidth:2});
</script>
