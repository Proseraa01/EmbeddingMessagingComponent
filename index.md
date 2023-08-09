<html>

  <body>
    <script type='text/javascript'>
    function initEmbeddedMessaging() {
        try {
            embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

            embeddedservice_bootstrap.init(
                '00DN0000000FH6T',
                'TestWebInApp',
                'https://gepuat--uat.sandbox.my.site.com/ESWTestWebInApp1691465770038',
                {
                    scrt2URL: 'https://gepuat--uat.sandbox.my.salesforce-scrt.com'
                }
            );
        } catch (err) {
            console.error('Error loading Embedded Messaging: ', err);
        }
    };
</script>
<script type='text/javascript' src='https://gepuat--uat.sandbox.my.site.com/ESWTestWebInApp1691465770038/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
  </body>
</html>

