# Einrichtung: To-dos über Kalender + Obsidian

**Prinzip:** Kalender = *wann*, Obsidian = *was & warum*. To-dos werden schnell gesammelt, beim Sortieren eingeordnet, und ein fester Kalendertermin führt dich zur Fokus-Notiz.

---

## 1. Dateien in den Vault legen (5 Min.)

| Datei | Wohin |
|---|---|
| `Inbox.md` | Vault-Hauptordner |
| `Fokus.md` | Vault-Hauptordner |
| `Vorlagen/Projekt.md` | in deinen Vorlagen-Ordner |

- Projekte kommen in einen Ordner **`Projekte`** (die Abfrage in `Fokus.md` sucht dort). Heißt dein Ordner anders, passe die Zeile `path includes Projekte` an.
- Vorlagen-Ordner eintragen: *Einstellungen → Kernplugins → Vorlagen → Speicherort*.

## 2. Tasks-Plugin installieren (2 Min.)

*Einstellungen → Community-Plugins → Durchsuchen → „Tasks“ → Installieren & Aktivieren.*

Danach zeigt `Fokus.md` automatisch die passenden Aufgaben an – egal in welcher Notiz sie stehen.

## 3. Kurzbefehl „Neues To-do“ (10 Min., einmalig)

Funktioniert auf iPhone **und** Mac (Kurzbefehle synchronisieren über iCloud). Obsidian öffnet sich kurz, die Notiz bleibt aber im Hintergrund.

Kurzbefehle-App → **+** → folgende Aktionen nacheinander:

1. **Nach Eingabe fragen** – Frage: `To-do?`
2. **Text** – Inhalt (wichtig: erste Zeile leer lassen, damit jedes To-do auf einer neuen Zeile landet):
   ```
   
   - [ ] [Angegebene Eingabe]
   ```
3. **URL-Codieren** – Eingabe: *Text*
4. **URL** – Inhalt:
   ```
   obsidian://new?vault=DEIN-VAULT-NAME&file=Inbox&append=true&silent=true&content=[URL-codierter Text]
   ```
   - `DEIN-VAULT-NAME` exakt so, wie der Vault in Obsidian heißt. Leerzeichen als `%20` schreiben (z. B. `Mein%20Vault`).
   - `[URL-codierter Text]` ist die Variable aus Schritt 3 (antippen und einfügen).
5. **URLs öffnen**

Name: **Neues To-do**. Dann:
- **iPhone:** zum Homescreen hinzufügen und/oder auf die Action-Taste legen. Per Siri: *„Neues To-do“*.
- **Mac:** im Kurzbefehl auf *ⓘ → Tastaturkurzbefehl hinzufügen*, z. B. `⌃⌥T`.

**Test:** Kurzbefehl ausführen, „Test“ eingeben → in `Inbox.md` steht `- [ ] Test`.

## 4. Fokus-Termin in Outlook (3 Min., einmalig)

- Neuer Termin, z. B. **Di 15:00–16:00**, Titel **„Fokus“**, als **Serie** (wöchentlich).
- Status: **Beschäftigt**. Eigene Farbkategorie „Fokus“.
- In der **Beschreibung** (nicht im Ort-Feld) den Link zur Fokus-Notiz einfügen:
  in Obsidian Rechtsklick auf `Fokus.md` → **„Obsidian-URL kopieren“**.
- Optional einen zweiten Block, z. B. Do vormittags.

Der Termin wird nie mehr angefasst. Was drin passiert, entscheidet die Fokus-Notiz.

## 5. Ablauf im Alltag

**Unterwegs (5 Sek.):** Kurzbefehl → To-do eintippen → fertig. Nicht nachdenken, nicht sortieren.

**Beim Sortier-Ritual (10 Min., z. B. Freitag oder Montag):** `Fokus.md` öffnen.
1. Inbox durchgehen: jedes To-do in die passende Projektnotiz unter *Nächster Schritt* verschieben (oder löschen, wenn es sich erledigt hat).
2. Unter *Nächste Schritte aus Projekten* **1–3 Aufgaben** auswählen und `#fokus` anhängen, z. B. `- [ ] Angebot Müller fertig machen #fokus`.
3. Mehr nicht. Was keinen `#fokus` bekommt, ist bewusst „nicht diese Woche“.

**Dienstag 15 Uhr:** Erinnerung → Link im Termin antippen → *Jetzt dran* zeigt dir, was zu tun ist. Erledigtes abhaken; es verschwindet automatisch.

**Abends (optional):** kurz im Verlauf der Projektnotiz notieren, was du geschafft hast. Das ist deine Done-Liste.

---

### Wenn es hakt
- **Fokus-Termin wird ständig überbucht:** auf eine Zeit legen, zu der selten Meetings sind (früh morgens oder freitags).
- **Zu viele #fokus-Aufgaben:** höchstens so viele markieren, wie in einen Block passen.
- **Kurzbefehl öffnet Obsidian nicht:** Vault-Name prüfen (Groß-/Kleinschreibung, `%20` statt Leerzeichen).
