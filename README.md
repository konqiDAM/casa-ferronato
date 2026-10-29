# Casa Ferronato — Website

Statische One-Page-Website für das Künstlerhaus Casa Ferronato in den Marken.

## Lokal ansehen

`index.html` im Browser öffnen. Für die Schriften wird eine Internetverbindung benötigt; die Bilder liegen lokal im Ordner `assets/`.

## Auf GitHub Pages veröffentlichen

1. Neues **öffentliches** Repository anlegen, z. B. `casa-ferronato`.
2. Remote hinzufügen und den vorhandenen Commit pushen:

   ```bash
   git remote add origin https://github.com/<benutzername>/casa-ferronato.git
   git push -u origin main
   ```

3. Im Repository: **Settings → Pages**.
4. Unter **Build and deployment** die Quelle **Deploy from a branch** wählen, Branch `main`, Ordner `/ (root)`, speichern.
5. Nach ein bis zwei Minuten ist die Seite unter `https://<benutzername>.github.io/casa-ferronato/` erreichbar.

## Eigene Domain

Im Repository unter **Settings → Pages → Custom domain** die Domain eintragen und speichern. GitHub legt dann eine `CNAME`-Datei an.

### Variante mit `www`

| Typ | Name | Wert |
| --- | --- | --- |
| CNAME | `www` | `<benutzername>.github.io` |

Die Apex-Domain (ohne `www`) beim Registrar auf `www` weiterleiten.

### Variante mit Apex-Domain

| Typ | Name | Wert |
| --- | --- | --- |
| A | `@` | `185.199.108.153` |
| A | `@` | `185.199.109.153` |
| A | `@` | `185.199.110.153` |
| A | `@` | `185.199.111.153` |
| CNAME | `www` | `<benutzername>.github.io` |

Nach der DNS-Einrichtung in GitHub **Enforce HTTPS** aktivieren. Bei Cloudflare die Einträge zunächst auf **DNS only** stellen.

## Noch zu ersetzen

- Die Platzhalter-Adresse `kontakt@casaferronato.example` im Kontaktbereich durch die echte E-Mail-Adresse ersetzen.
- Optional: eine `CNAME`-Datei mit der Wunschdomain anlegen.
