---
sidebar_position: 2
---

# Testing

Eine kurze Anleitung um deine Ionic App auf einem Android oder IOS Device zu testen.

## Android Testing

**Wenn du deine App für Android testen willst gibt es 2 Möglichkeiten, entweder testest du die App auf einem virtuellen oder einem physischen Device in Android Studio.**

1. Android Dateien über den Capacitor erstellen lassen.
```bash
ionic capacitor build android
```

2. Falls die Path variable für Android Studio richtig gesetzt ist, öffnet sich Android Studio von selbst. Sollte das nicht der Fall sein, öffne den erstellten Ordner ('android') in Android Studio.

3. Ab hier muss zwischen den beiden Methoden unterschieden werden.
    - **Über ein virtuelles Device Testen.**
        1. Navigiere auf der rechten Seite mit dem `Device Manager` auf `Add a new device` und dann auf `Create Virtual Device`.

           ![](https://api.heedix.de/v1/images/33af1907-45d6-4f37-8065-b621d39dada1.png?size=large)

        2. Nun kannst du dir ein Device deiner Wahl aussuchen, auf dem du die App testen willst.

           ![](https://api.heedix.de/v1/images/be1a14cc-42af-437d-ab9c-244029b5ae7d.png?size=large)

        3. Nachdem du ein Device gewählt hast, kannst du noch ein Android Version wählen (Hier ist es empfohlen einfach die dem Device zugehörige Version beizubehalten).

           ![](https://api.heedix.de/v1/images/1a7dc47d-37d7-47d6-943f-a9ea56d44cc1.png?size=large)

        4. Zum Schluss kannst du dem Device noch einen Namen geben.

           ![](https://api.heedix.de/v1/images/3eef651d-24cb-41f8-802c-a95e8453831c.png?size=large)

        5. Anschließend kannst du das Device entweder direkt über den `Run` Button in Android Studio starten, oder das Device im Device Manager starten und anschließend die App über den `Run` Button in Android Studio starten. Die App kann auch anschließend mit dem gleichen Button Restarten

           ![](https://api.heedix.de/v1/images/fc233e47-3bbe-4801-a8f8-e1c6fd54cc38.png?size=large)

    - **Über ein physisches Device testen**
        1. Du musst auf dem remote Device unter `Einstellungen > Entwickleroptionen > USB-Debugging` aktiviert haben.
        2. Schließe jetzt dein Device über USB an.
        3. Auf deinem Device sollte eine Meldung kommen, die du akzeptieren musst.
        4. Wenn du das getan hast, taucht in deinem Android Studio das Remote Device auf. Dieses kannst du jetzt über den `Start Mirroring` Button starten.

           ![](https://api.heedix.de/v1/images/6db17542-a129-4a74-8818-58d008bae0e5.png?size=large)

        5. Sobald das Device gestartet ist, kannst du die App über den Start Button in Android Studio starten.

           ![](https://api.heedix.de/v1/images/fc233e47-3bbe-4801-a8f8-e1c6fd54cc38.png?size=large)

        6. Nun kannst du die App auf deinem physischen Device testen.

           ![](https://api.heedix.de/v1/images/e2a2002d-9efa-4344-962e-c480e57fa6be.png?size=large)

## IOS Testing

**⚠️ Um eine IOS App zu testen benötigst du einen Computer mit macOS.**

1. IOS Dateien über den Capacitor erstellen lassen.
```bash
ionic capacitor build ios
```

2. Nun sollte ein ordner namens `ios` mit der App als native IOS App. Diesen ordner kannst du jetzt in Xcode öffnen.
3. Wenn du die App in Xcode geöffnet hast, solltest du diese über den `Build and Run` Button ausführen können. Neben diesem Button kannst du zudem ein Device auswählen welches Emuliert werden soll.

   Wenn du ein IOS Gerät per USB angeschlossen hast, kannst du dieses ebenfalls auswählen um die App zu runnen.

   ![](https://docs-assets.developer.apple.com/published/c78867b72637128da112da32fb68b9c8/build-hero-window~dark@2x.png)