<head>

 <script src="https://cdn.onesignal.com/sdks/OneSignalSDK.js" async=""></script>
<script>
   var OneSignal = window.OneSignal || [];
    var initConfig = {
        appId: "5b5be79a-c8b9-4458-8ea6-ad1170a06e1e",
        notifyButton: {
            enable: true
        },
    };
    OneSignal.push(function () {
        OneSignal.SERVICE_WORKER_PARAM = { scope: '/web/OneSignal-Web-SDK-HTTPS-Integration-Files/' };
        OneSignal.SERVICE_WORKER_PATH = '/web/OneSignal-Web-SDK-HTTPS-Integration-Files//OneSignalSDKWorker.js'
        OneSignal.SERVICE_WORKER_UPDATER_PATH = '/web/OneSignal-Web-SDK-HTTPS-Integration-Files//OneSignalSDKUpdaterWorker.js'
        OneSignal.init(initConfig);
    });
 
OneSignal.push(function() {
  OneSignal.isPushNotificationsEnabled().then(function(isEnabled) {
    if (isEnabled)
  
      open(location, '_self').close();
    else
      console.log("Push notifications are not enabled yet.");      
  });
});
 
</script>
  
  
  
  

  
</head>
<body>
  After you accept subscriptions, come on back!</body>

