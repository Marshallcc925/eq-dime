# EQ Dime

Ecualizador de 10 bandas con reproductor local. Web Audio API + Capacitor.

## Opcion A: APK sin instalar nada (GitHub Actions)
1. Cree un repositorio en GitHub y suba todo el contenido de esta carpeta.
2. Pestana Actions > Build APK > espere a que termine (3 a 5 min).
3. Abra la ejecucion y descargue el artefacto EQ-Dime-apk. Dentro esta app-debug.apk.
4. Pase el APK al Samsung (USB, Drive o WhatsApp), toquelo y permita "Instalar apps desconocidas".

## Opcion B: compilar en su laptop
Requisitos: Node 18+, JDK 17, Android Studio (SDK).
    npm install
    npx cap add android
    npx cap sync android
    cd android && ./gradlew assembleDebug
APK: android/app/build/outputs/apk/debug/app-debug.apk
(o `npx cap open android` y Run desde Android Studio)

## Probar rapido en el navegador
    npx serve www
