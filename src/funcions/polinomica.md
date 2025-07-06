# Funció polinòmica

Una funció polinòmica és una funció de la forma:

\\[
f(x) = a_n x^n + a_{n-1} x^{n-1} + \cdots + a_1 x + a_0
\\]

on \\(a_0, a_1, \dots, a_n\\) són coeficients reals i \\(n\\) un enter no negatiu que indica el grau del polinomi.


## Tipus de polinomis

- **Polinomi de grau 2 (quadràtic):**

\\[
f(x) = a x^2 + b x + c
\\]

Exemple: \\(f(x) = 2x^2 - 3x + 1\\).

- **Polinomi de grau 3 (cúbic):**

\\[
f(x) = a x^3 + b x^2 + c x + d
\\]

Exemple: \\(f(x) = x^3 - 2x^2 + x - 5\\).

- **Polinomi de grau \\(n\\) (general):**

\\[
f(x) = \sum_{k=0}^n a_k x^k
\\]


## Domini

El domini d’una funció polinòmica és tot \\( \mathbb{R} \\), ja que està definida per a tots els valors reals.


<div id="jxgbox" class="jxgbox" style="width:600px; height:300px;"></div>

<script>
var board = JXG.JSXGraph.initBoard('jxgbox', {
  boundingbox: [-2, 10, 4, -10],
  axis: true,
  pan: { enabled: true, needTwoFingers: false, needShift: false },
  zoom: { enabled: true, factorX: 1.25, factorY: 1.25, wheel: true, needShift: false },
  showCopyright: false
});
var f = board.create('functiongraph', function(x) {
  return x*x*x - 3*x*x + 2;
}, {strokeColor: '#0077CC', strokeWidth: 2});
</script>
