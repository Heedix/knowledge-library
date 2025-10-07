---
sidebar_position: 3
---

# Deployment

Eine kurze Anleitung um deine Ionic App als Android oder IOS App zu deployen.

**⚠️ Android wurde von mir bereits getestet und funktioniert bei IOS hab ich bis jetzt nur einen Link und eine Beschreibung eingefügt, ob das funktioniert weiß ich noch nicht.**

## Android deployment

1. Android Dateien über den Capacitor erstellen lassen.
```bash
ionic capacitor build android
```

2. Falls die Path variable für Android Studio richtig gesetzt ist, öffnet sich Android Studio von selbst. Sollte das nicht der Fall sein, öffne den erstellten Ordner ('android') in Android Studio.
3. Jetzt kannst du unter dem Reiter `Build > Build App Bundle(s) / APK(s) > Build APK(s)` das Projekt als APK builden lassen.

   ![](https://api.heedix.de/v1/images/6c3cea4c-37a1-4869-8882-d6b9abaec8f8.png?size=large)

4. Die erstellte Datei findest du unter `\android\app\build\outputs\apk\debug`
    - Die Datei sollte `app-debug.apk` heißen
    - Diese Datei kannst du nun auf dein Handy laden und ausführen. Dadurch wird die App automatisch installiert und du kannst sie verwenden.

## IOS deployment

**⚠️ Um eine IOS App zu deployen benötigst du einen Computer mit macOS.**

1. IOS Dateien über den Capacitor erstellen lassen.
```bash
ionic capacitor build ios
```

2. Nun sollte ein ordner namens `ios` mit der App als native IOS App. Diesen ordner kannst du jetzt in Xcode öffnen.
3. Jetzt solltest du ein IOS Gerät mit deinem Computer verbinden.
4. Wähle dieses Gerät in der oberen leiste aus und Klicke anschließend auf `Build and Run`

   ![](https://docs-assets.developer.apple.com/published/c78867b72637128da112da32fb68b9c8/build-hero-window~dark@2x.png)

5. Die App sollte sich jetzt automatisch auf dem angeschlossenen Gerät installieren