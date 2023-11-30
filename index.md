<html>

  <body>
    <script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
            window.addEventListener("onEmbeddedMessagingReady", () => {     
            console.log( "Inside Prechat API!!" ); 
             embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields( { "First_Name" : "Anuj","Last_Name" : "Kumar","Email" : "upendra.singh@proseraa.com","Client Name" : "ChevronTraining4","Client User Type" : "Buyer" } );
              });
			embeddedservice_bootstrap.init(
				'00DN0000000FH6T',
				'SmartLocal',
				'https://gepuat--uat.sandbox.my.site.com/ESWSmartLocal1700214312423',
				{
					scrt2URL: 'https://gepuat--uat.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://gepuat--uat.sandbox.my.site.com/ESWSmartLocal1700214312423/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
  </body>
</html>

