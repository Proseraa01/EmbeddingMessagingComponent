<html>
<body>
  <!-- Begin Default Content REMOVE THIS -->
  <h1>Congratulations</h1>
<style type='text/css'>
     .embeddedServiceHelpButton{
           .embeddedServiceHelpButton .helpButton .uiButton{
            background-color:#fa6400;
            font-family:"Arial",sans-serif;
            border-radius:23px;
            min-width:10em;
            max-width:10em
            }
            .embeddedServiceHelpButton .embeddedServiceIcon{
            display:none!important;
            }
            .helpButtonLabel .message{
            background-color: #fa6400;
            border: none;
            color: white;
            font-weight: bold;
            font-size: 12px;
            }
</style>
<script type='text/javascript' src='https://service.force.com/embeddedservice/5.0/esw.min.js'></script>
<script type='text/javascript'>
    var initESW = function(gslbBaseURL) {
        embedded_svc.settings.displayHelpButton = true; //Or false
        embedded_svc.settings.language = ''; //For example, enter 'en' or 'en-US'

        embedded_svc.settings.defaultMinimizedText = 'Chat'; //(Defaults to Chat with an Expert)
        //embedded_svc.settings.disabledMinimizedText = '...'; //(Defaults to Agent Offline)

        //embedded_svc.settings.loadingText = ''; //(Defaults to Loading)
        //embedded_svc.settings.storageDomain = 'yourdomain.com'; //(Sets the domain for your deployment so that visitors can navigate subdomains during a chat session)

        // Settings for Chat
        //embedded_svc.settings.directToButtonRouting = function(prechatFormData) {
            // Dynamically changes the button ID based on what the visitor enters in the pre-chat form.
            // Returns a valid button ID.
        //};
        //embedded_svc.settings.prepopulatedPrechatFields = {}; //Sets the auto-population of pre-chat form fields
        //embedded_svc.settings.fallbackRouting = []; //An array of button IDs, user IDs, or userId_buttonId
        //embedded_svc.settings.offlineSupportMinimizedText = '...'; //(Defaults to Contact Us)
        embedded_svc.settings.chatbotAvatarImgURL = "https://duroflexpvtltd.my.salesforce-sites.com/resource/SleepyheadLogo";
        embedded_svc.settings.enabledFeatures = ['LiveAgent'];
        embedded_svc.settings.entryFeature = 'LiveAgent';
        embedded_svc.settings.extraPrechatFormDetails = [{
  "label":"First Name", 
  "transcriptFields": ["First_Name__c"]
},{
  "label":"Last Name", 
  "transcriptFields": ["Last_Name__c"]
},{
  "label":"Phone", 
  "transcriptFields": ["Customer_Mobile_Number__c"]
}
,{
  "label":"Customer Email", 
  "transcriptFields": ["Customer_Email__c"]
}
,{
  "label":"Subject", 
  "transcriptFields": ["Issue__c"]
}
];

        embedded_svc.init(
            'https://duroflexpvtltd.my.salesforce.com',
            'https://duroflexpvtltd.my.site.com/',
            gslbBaseURL,
            '00D2w00000MhMkY',
            'WhatsappBot_Deployment',
            {
                baseLiveAgentContentURL: 'https://c.la2-c2-ukb.salesforceliveagent.com/content',
                deploymentId: '5722w000000ZLJl',
                buttonId: '5732w000000DR5T',
                baseLiveAgentURL: 'https://d.la2-c2-ukb.salesforceliveagent.com/chat',
                eswLiveAgentDevName: 'EmbeddedServiceLiveAgent_Parent04I2w0000008ioNEAQ_18ba3a93ef5',
                isOfflineSupportEnabled: false
            }
        );
    };

    if (!window.embedded_svc) {
        var s = document.createElement('script');
        s.setAttribute('src', 'https://duroflexpvtltd.my.salesforce.com/embeddedservice/5.0/esw.min.js');
        s.onload = function() {
            initESW(null);
        };
        document.body.appendChild(s);
    } else {
        initESW('https://service.force.com');
    }
</script>
</body></html>
