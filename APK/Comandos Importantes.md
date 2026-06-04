### ionic capacitor run android -l

```bash
ionic capacitor run ios --livereload
ionic capacitor run android -l --external
ionic capacitor run android -l --open --external
ionic capacitor sync
ionic capacitor open android
ionic capacitor platform rm android
ionic capacitor platform add android
ionic capacitor platform prepare android
ionic capacitor build android --configuration=test
ionic capacitor run android --configuration=test -l --open --external
```

### Verificar firma APK
```bash
keytool -printcert -jarfile ApkAnalizamos.v.1.9.0.apk
```

### Ruta MainActivity
```
Src/main/java/crezcamos/analizamos/MainActivity.java
```

### Código FLAG_SECURE
```java
getWindow().setFlags(WindowManager.LayoutParams.FLAG_SECURE, 
                     WindowManager.LayoutParams.FLAG_SECURE);
```

## 1. Levantar el servidor (en VS Code)
```bash
ionic capacitor run android -l --open
```

## 2. Conectar el puerto (en terminal de Android Studio)
```bash
"/d/Program Files/Android/SDKinstall/platform-tools/adb" reverse tcp:8100 tcp:8100
```

## 3. Simular GPS (opcional)
```bash
"/d/Program Files/Android/SDKinstall/platform-tools/adb" emu geo fix -73.1198 7.1193
```

![[GetImage.png]]