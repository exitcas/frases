# [Las Frases&trade;](/)

## Cargar frase
<style>
  .fr{font-size:larger;font-weight:bold;font-family:serif;border:none;}
</style>
<form method="POST">
  <div id="error">{{error}}</div>
  <p><span class="fr">"<input id="principal_input" class="fr" style="" type="text" name="frase" placeholder="Frase" />"</span><br />--<input style="border:none" type="text" name="nombre" placeholder="Nombre (opcional)" /><br /><input type="submit" value="Sugerir" /></p>
  <p>*la frases se aprueban manualmente</p>
</form>
<script>
  document.getElementById("principal_input").style = "width:100px";
  document.getElementById("principal_input").onkeypress = function(event) {
    var val = document.getElementById("principal_input").value;
    document.getElementById("principal_input").style = "width:" + (val.split("").length * 20).toString() + "px";
  }
</script>

&copy;2022 [ATICO.ga](https://atico.ga)