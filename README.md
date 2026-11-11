# JARVIS Backup – öffentliche OAuth-Informationsseite

Dieses **öffentliche Repository** enthält ausschließlich eine statische Informationsseite für die private Anwendung **JARVIS Backup**.

**Keine** Google-OAuth-Tokens, rclone-Konfigurationsdateien, Passwörter, Recovery-Schlüssel, Serveradressen, VM-Archive, Sicherungsmetadaten oder private Infrastruktur-Dokumentation hier ablegen.

## Inhalt
- `index.html`: App-Startseite
- `privacy.html`: eigene Datenschutzerklärung
- `terms.html`: eigene Nutzungsbedingungen
- `style.css`: Styling ohne externe Ressourcen

## GitHub Pages aktivieren
Im Repository: **Settings → Pages → Build and deployment → Deploy from a branch → main → /(root) → Save**.

Nach erfolgreichem Deployment voraussichtliche öffentliche URLs:
- `https://ferngro.github.io/Jarvis_Backup_Google_Cloud/`
- `https://ferngro.github.io/Jarvis_Backup_Google_Cloud/privacy.html`
- `https://ferngro.github.io/Jarvis_Backup_Google_Cloud/terms.html`

**Diese URLs erst nach tatsächlich erfolgreicher Pages-Veröffentlichung in Google OAuth eintragen.** GitHub Pages wird nicht durch das bloße Hochladen der Dateien automatisch freigeschaltet.

## Google OAuth
In **Google Cloud Console → Google Auth Platform → Branding** müssen die URLs zur tatsächlichen App und zur echten Datenschutzerklärung gehören. Nicht das GitHub-Profil oder die Datenschutzseite von GitHub selbst verwenden. Die Zulässigkeit von `github.io` als autorisierte Domain hängt von der konkreten Google-OAuth-Verifikationsprüfung ab; im Fall formeller Domainverifikation kann eine eigene kontrollierte Domain erforderlich sein. Danach in **Zielgruppe** veröffentlichen und erst dann auf Proxmox den bestehenden rclone-Remote neu autorisieren.

Datenverarbeitungsinformationen regelmäßig mit dem tatsächlich angeforderten Google-Drive-OAuth-Scope und der eingesetzten Restic-/rclone-Konfiguration abgleichen.

Das eigentliche private Infrastruktur-Repository und der Memory Vault bleiben **separat und privat**.
