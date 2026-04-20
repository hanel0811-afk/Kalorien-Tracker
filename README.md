# 🥗 Kalorien-Tracker mit Firebase

Foto-Upload-App mit Firebase Storage + Netlify (100% kostenlos)

## 📦 Setup

### 1. Firebase Config
Speicher deine `firebase-config.js` im selben Ordner wie `index.html`:

```javascript
// firebase-config.js
const firebaseConfig = {
  apiKey: "...",
  authDomain: "...",
  projectId: "...",
  storageBucket: "...",
  messagingSenderId: "...",
  appId: "..."
};
```

### 2. Lokal testen
```bash
# Mit Live Server (VS Code Extension) oder einfach:
# Öffne index.html im Browser
```

### 3. Auf Netlify deployen (kostenlos!)

**Option A: Drag & Drop (am einfachsten)**
1. Geh zu [netlify.com](https://netlify.com)
2. Melde dich an (mit GitHub oder Email)
3. Zieh den `Kalorien-Tracker` Ordner auf die Seite
4. Fertig! 🎉

**Option B: Mit Git (GitHub)**
1. Erstelle GitHub Repo
2. Push deine Dateien
3. Verbinde mit Netlify
4. Auto-Deploy ✅

## 🔒 Firebase Sicherheit

Die `firebase-config.js` enthält deine Firebase Keys. 
⚠️ **WICHTIG:** 
- Nie ins Git committen (`.gitignore` ist gesetzt)
- Testmodus sollte aktiviert sein (kostenlos!)
- Später Firestore Regeln anpassen

Aktuelle Rules (Testmodus):
```
allow read, write: if request.auth != null;
```

## 📊 Kostenlos Limits

- Storage: 5 GB kostenlos
- Downloads: 1 GB/Tag kostenlos
- Uploads: Unbegrenzt im kostenlosen Plan

## 🚀 Troubleshooting

**"CORS Error"** → Firebase Storage braucht richtige Sicherheitsregeln
**"Fotos laden nicht"** → Check Firebase Console > Storage > Permissions
**"Upload geht nicht"** → Testmodus aktiviert? Rules richtig?

## 📝 Nächste Schritte

- [ ] Foto-Metadaten speichern (Firestore)
- [ ] Benutzer-Authentifizierung
- [ ] Kategorien/Mahlzeiten
- [ ] Statistiken anzeigen

---
**Brauchst du Hilfe?** Frag Claude! 🤖
