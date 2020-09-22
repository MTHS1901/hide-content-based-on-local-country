# HIDE HTML CONTENT IN A SPECIFIC PARENT OR STATE
HTML + Javascript (jquery) to hide a div in a specific country.

#### API: https://freegeoip.app/
#### Jquery: https://code.jquery.com/

### PLAY WITH THE CODE HERE: https://www.w3schools.com/code/tryit.asp?filename=GDWGAD4FTESB

### EXAMPLE:
##### Note: the country is defined by two acronyms eg BRAZIL = BR, UNITED STATES = US, see: https://www.iban.com/country-codes, you can also hide the content in a STATE specific using "(data.region_code == 'SP')" // hidden in São Paulo.

#### You can create your own COUNTRY and STATE variables using SCRIPT's IF and ELSE.

Example:

``
<html>
<script src = "https://code.jquery.com/jquery-3.5.0.min.js" integrity = "sha256-xNzN2a4ltkB44Mc / Jz3pT4iU1cmeR0FkXs4pru / JxaQ =" crossorigin = "anonymous"> </script>
<div id = "content">
<p> YOU'RE SEEING THIS WHY YOU ARE IN BRAZIL </p>
</div>
<script>
$ (function () {
    $ .getJSON ('https://freegeoip.app/json/', function (data) {
        if (data.country_code == 'BR') {
            $ ('# content'). show ();
        } else {
            $ ('# content'). fadeOut ();
        }
    });
});
</script>
</html>
``

by MTHS1901 - www.mths1901.com
