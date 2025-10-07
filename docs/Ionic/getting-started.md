---
sidebar_position: 1
---

# Getting started

Eine kurze Anleitung um mit Ionic und React zu starten.

## Voraussetzungen

- Node.js inklusive npm muss installiert sein.

## Installation

1. Installiere ionic-cli und capacitor.
```bash
npm install -g @ionic/cli @capacitor/assets
```

2. installiere React-Dom.
```bash
npm install react react-dom
```

3. Anpassung der ExecutionPolicy um RemoteSigned Packages zuzulassen.
    - Mit der Einstellung RemoteSigned dürfen lokal erstellte Skripte ohne Signatur ausgeführt werden.
    - ⚠️ **Achtung:**  muss nur gemacht werden, wenn Befehle wie `ionic --version` nicht  funktionieren.
```powershell
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
```

4. Für das Deployen/Testen einer Android-App muss [Android Studio](https://developer.android.com/studio?hl=de) installiert sein.
5. Für das Deployen/Testen einer IOS App benötigt man einen macOS Computer auf dem [Xcode](https://apps.apple.com/de/app/xcode/id497799835) installiert ist.

## Projekt starten

1. Ionic Projekt initialisieren.
    - [Templates](https://javascript.plainenglish.io/the-different-types-of-ionic-5-starter-template-75091ae916e3)
```bash
ionic start {{Projekt-Name}} {{Template}} --type=react --capacitor
```

2. App runnen.
    - Hiermit siehst du ein Preview deiner App im Browser.
```bash
ionic serve
```