Goo Pro - Build & Release Guide (EN & AR)

(EN)
1) Prepare environment: Flutter SDK, Java JDK, Android SDK.
2) Create a signing keystore.
3) Add keystore to GitHub Secrets as KEYSTORE_BASE64 and other secrets.
4) Use GitHub Actions to build signed AABs.
5) Upload AABs to Google Play Console.

(AR)
1) تأكد من تنصيب: Flutter SDK، Java JDK، Android SDK.
2) أنشئ keystore:
   keytool -genkey -v -keystore ~/goo_pro_key.jks -alias goo_pro_key -keyalg RSA -keysize 2048 -validity 10000
3) قم بترميز الملف base64 وادخاله كـ SECRET في GitHub.
4) اضف الأسرار في Settings -> Secrets في GitHub repository.
5) شغّل workflow وستنتج AABs كمخرجات.
