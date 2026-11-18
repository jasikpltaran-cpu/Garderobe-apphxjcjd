# Гардероб: збірка APK

## Найпростіше: GitHub (без Android Studio)
1. Створіть безкоштовний акаунт на github.com і новий репозиторій.
2. Завантажте в нього вміст цієї папки (Add file, Upload files). Папка .github має потрапити в репозиторій.
3. Відкрийте вкладку Actions, оберіть «Build APK» і натисніть Run workflow.
4. Через 5–10 хвилин відкрийте завершений запуск і завантажте архів garderob-apk. Усередині app-debug.apk.
5. Перекиньте APK на телефон і встановіть (дозвольте встановлення з невідомих джерел).

## Альтернатива: на комп’ютері
Потрібні Node.js 20, JDK 17 і Android Studio.
    npm install
    npx cap add android
    (додайте дозволи CAMERA, ACCESS_FINE_LOCATION, ACCESS_COARSE_LOCATION в android/app/src/main/AndroidManifest.xml)
    npx cap sync android
    npx cap open android   (Build, Build APK)
