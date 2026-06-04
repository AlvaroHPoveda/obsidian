## Fix BarcodeScanner Build Error

**Referencia:** [Ionic Forum - Error build phonegap-barcodescanner](https://forum.ionicframework.com/t/error-when-i-build-with-phonegap-barcodescanner-ionic-native/218337/5)

**Agregar en** `build.gradle`:

```gradle
apply from: "../../node_modules/phonegap-plugin-barcodescanner/src/android/barcodescanner.gradle"
```