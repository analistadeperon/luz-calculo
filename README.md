# luz-calculo
<div id="app"></div>

<html>
<body>
<script>

var consumo=parseFloat(prompt("digite o consumo:"));
var watt;
 
 if(consumo<100) {
  document.write ("<p>Categoria A");
  watt=0.0003;
  
 }
 else if(consumo>100 && consumo<=300) {
  document.write ("<p>Categoria B");
  watt=0.0005;
 }
 else if(consumo>300 && consumo<=600) {
  document.write ("<p>Categoria C");
  watt=0.0008;
 }
 else{
  document.write ("Categoria D");
  watt=0.0012;
 }
 
 var vb=consumo*1000*watt;
  document.write ("<p>Valor bruto= R$ " +vb);
  
 var ipi=vb*0.29;
  document.write ("<p> Valor do IPI: R$ " +ipi);
  
 var icms= (vb/(100-24)*0.24)*100;
  document.write ("<p> Valor do ICMS: R$ " +icms);
  
 var tp=(vb+ipi+icms);
  document.write ("<p> Valor total a pagar: R$ " +tp);
 
 
</script>
</body>
</html>
