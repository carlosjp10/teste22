<html>
    <body>
        <script type='text/javascript'>
    function initEmbeddedMessaging() {
        try {
            embeddedservice_bootstrap.settings.language = 'pt_BR'; // For example, enter 'en' or 'en-US'

            embeddedservice_bootstrap.init(
                '00DDw000005FD1I',
                'WebChatFSRental',
                'https://page-connect-8459--dev.sandbox.my.site.com/ESWWebChatFSRental1706116958228',
                {
                    scrt2URL: 'https://page-connect-8459--dev.sandbox.my.salesforce-scrt.com'
                }
            );
        } catch (err) {
            console.error('Error loading Embedded Messaging: ', err);
        }
    };
</script>
<script type='text/javascript' src='https://page-connect-8459--dev.sandbox.my.site.com/ESWWebChatFSRental1706116958228/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
    </body>
</html>
