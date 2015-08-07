# Scripts
In the next lines we want to explain the different scripts in this repository and their utility.
## download_androguard_report.py
This script, giving a sha256 hash download the androguard report from Koodous.

The report format is like the next one:
```
{
    "app_name": "WhatsApp",
    "package_name": "com.whatsapp.downloader",
    "providers": [
    ],
    "new_permissions": [
    ],
    "filters": [
        "android.intent.action.MAIN"
    ],
    "max_sdk_version": null,
    "certificate": {
        "sha1": "B55451A7B307642EF6A0680F979CFB80DE0D91A1",
        "IssuerDN": "CN=MobileAZ",
        "subjectDN": "CN=MobileAZ"
    },
    "min_sdk_version": null,
    "version_code": "1",
    "libraries": [
    ],
    "target_sdk_version": null,
    "cordova": null,
    "activities": [
        "vn.vimob.Vimob",
        "vn.payment.purchase",
        "com.google.android.gms.ads.AdActivity"
    ],
    "main_activity": "vn.vimob.Vimob",
    "receivers": [
        "vn.receiver.callReceiver",
        "vn.receiver.screenReceiver",
        "vn.receiver.bootReceiver"
    ],
    "signature_name": "META-INF/CERT.RSA",
    "dexes": {
        "classes": {
            "ssdeep": "49152:Va27c4iWbnQcJfnqpLAcofnfl1tncJVkOho17MnsEI6VIcS:lo4L8c6Acq17M",
            "sha256": "683b22d1ab311565b00a15957c1ae29ad566ce153bb79a230ea9bb451575f7c5"
        }
    },
    "displayed_version": "1.0",
    "services": [
    ],
    "permissions": [
        "android.permission.VIBRATE",
        "android.permission.RECEIVE_BOOT_COMPLETED",
        "android.permission.INTERNET",
        "android.permission.SYSTEM_ALERT_WINDOW",
        "android.permission.SEND_SMS",
        "android.permission.PROCESS_OUTGOING_CALLS",
        "android.permission.ACCESS_NETWORK_STATE",
        "android.permission.WAKE_LOCK",
        "android.permission.READ_PHONE_STATE",
        "android.permission.WRITE_EXTERNAL_STORAGE"
    ],
    "functionalities": {
        "ads": [
            {
                "code": "const-class v0, Lcom/google/ads/mediation/admob/AdMobAdapter;",
                "class": "Lcom/google/android/gms/ads/AdRequest$Builder;",
                "method": "addNetworkExtrasBundle"
            },
            {
                "code": "const-class v2, Lcom/google/ads/mediation/admob/AdMobAdapter;",
                "class": "Lcom/google/android/gms/ads/internal/client/zzg;",
                "method": "zza"
            },
            {
                "code": "instance-of v0, v3, Lcom/google/android/gms/ads/mediation/admob/AdMobExtras;",
                "class": "Lcom/google/android/gms/ads/internal/client/zzx$zza;",
                "method": "zza"
            }
        ],
        "SMS": [
            {
                "code": "invoke-virtual/range v0 ... v5, Landroid/telephony/SmsManager;->sendTextMessage(Ljava/lang/String; Ljava/lang/String; Ljava/lang/String; Landroid/app/PendingIntent; Landroid/app/PendingIntent;)V",
                "class": "Lcom/paygol/sdk/PayGolSDKPayment;",
                "method": "sendSMSMessages"
            }
        ]
    },
    "urls": [
        "https://www.linkedin.com",
        "google.com/iid",
        "http://www.paygol.com/ws/mobile/request",
        "https://www.googleapis.com/auth/games",
        "https://www.google-analytics.com",
        "http://www.paygol.com/ws/mobile/test",
        "https://www.googleapis.com/auth/fitness.nutrition.write",
        ...
    ]
}


```