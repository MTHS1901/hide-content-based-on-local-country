# OCULTAR CONTEUDO HTML EM UM PAIS ESPECIFICO
HTML + Javascript (jquery) para ocultar uma div em um pais especifico.

#### API: https://freegeoip.app/
#### Jquery: https://code.jquery.com/

### BRINQUE COM O CODIGO AQUI: https://www.w3schools.com/code/tryit.asp?filename=GDWGAD4FTESB
### EXEMPLO:
##### Nota: o pais é definido por duas siglas ex: BRASIL= BR, ESTADOS UNIDOS= US, veja: https://www.iban.com/country-codes
```
<html>
<script src="https://code.jquery.com/jquery-3.5.0.min.js" integrity="sha256-xNzN2a4ltkB44Mc/Jz3pT4iU1cmeR0FkXs4pru/JxaQ=" crossorigin="anonymous"></script>
<div id="conteudo">
<p> VOCÊ ESTÁ VENDO ISSO POR QUE ESTÁ NO BRASIL </p>
</div>
<script>
$(function() {
    $.getJSON('https://freegeoip.app/json/', function(data) {
    // CODIGO DO PAIS DEFINIDO COM DUAS SIGLAS (ex: BRASIL= BR, ESTADOS UNIDOS= US)
        if (data.country_code == 'BR') {
            $('#conteudo').show();
        }else{
            $('#conteudo').fadeOut();
        }
    });
});
</script>
</html>
´´´´
## Duvidas? www.mths1901.com/suporte
