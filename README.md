# Rhythm Tap — сборка APK
Вариант 1 (без установки Android Studio): залейте папку в GitHub-репозиторий -> Actions -> Build APK -> скачайте app-debug.apk из Artifacts.
Вариант 2 (локально, нужны Node 18+, JDK 17, Android SDK):
  npm install && npx cap add android && npx cap sync android
  cd android && ./gradlew assembleDebug
  APK: android/app/build/outputs/apk/debug/app-debug.apk
Правки игры вносятся в www/index.html, затем `npx cap sync android` и пересборка.
