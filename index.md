<html>
  <body>
    <script type='text/javascript'>
        var ipUser = "001.112.254.889";
        var buttomChat = '225569';
        
    function initEmbeddedMessaging() {
        try {
            embeddedservice_bootstrap.settings.language = 'pt_BR'; // For example, enter 'en' or 'en-US'
            
          window.addEventListener("onEmbeddedMessagingReady", () => {
            console.log("Received the onEmbeddedMessagingReady event…444");

            // Send data to Salesforce
            embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({
                "IpUsuario" : ipUser,
                "Idioma" : 'Português';
            });

            // Remove any items from the previous list that you don't want to send
            //embeddedservice_bootstrap.prechatAPI.removeHiddenPrechatFields(["Customer_ID"]);
            });
            
            embeddedservice_bootstrap.init(
                '00DDH00000057zF',
                'Messaging_Teste',
                'https://h2club--multiedro.sandbox.my.site.com/ESWMessagingTeste1702039722929',
                {
                    scrt2URL: 'https://h2club--multiedro.sandbox.my.salesforce-scrt.com'
                }
            );
        } catch (err) {
            console.error('Error loading Embedded Messaging: ', err);
        }
    };
    </script>
    <script type='text/javascript' src='https://h2club--multiedro.sandbox.my.site.com/ESWMessagingTeste1702039722929/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
  </body>
</html>
