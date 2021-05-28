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
        OneSignal.SERVICE_WORKER_PARAM = { scope: '/push/onesignal/' };
        OneSignal.SERVICE_WORKER_PATH = 'push/onesignal/OneSignalSDKWorker.js'
        OneSignal.SERVICE_WORKER_UPDATER_PATH = 'push/onesignal/OneSignalSDKUpdaterWorker.js'
        OneSignal.init(initConfig);
    });
</script>
  
</head>
<body>
  After you accept subscriptions, come on back!</body>

