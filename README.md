# AC News · AlveroCity

Eine News-Website für AlveroCity mit Registrierung, öffentlicher Startseite und geschützter Redaktion.

## Starten

```powershell
node server.js
```

Danach im Browser `http://localhost:3000` öffnen.

## Erster Zugang

- Benutzername: `admin`
- Passwort: `ACNews1`

Alle Besucher müssen sich beim ersten Aufruf registrieren oder anmelden. Nur Konten mit der Rolle Admin sehen den Redaktionszugang. Setze vor einer öffentlichen Bereitstellung unbedingt die Umgebungsvariable `ADMIN_PASSWORD`; Beiträge und Konten liegen anschließend dauerhaft in `data.json`. Diese Datei enthält Passwort-Hashes, niemals Klartextpasswörter. Für eine öffentliche Bereitstellung sollte die Anwendung hinter HTTPS und einem Reverse Proxy laufen.
