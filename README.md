# Spieltimer P2P (v1.5)
**by Sascha Urban**

Ein Mehrspieler-Zugtimer für Brett- und Gesellschaftsspiele. Läuft komplett im Browser, keine Installation nötig!

## Download Anleitungen
- [Ausführliche Bedienungsanleitung (PDF)](https://github.com/sasurb/spieltimer/raw/main/Bedienungsanleitung.pdf)
- [Schnellanleitung (PDF)](https://github.com/sasurb/spieltimer/raw/main/Schnellanleitung.pdf)

---

## 1. Die Lobby (Vorbereitung)

### Raum erstellen (Host)
1. Rufe die Webseite auf: [https://sasurb.github.io/spieltimer/](https://sasurb.github.io/spieltimer/)
2. Gib deinen Namen ein.
3. Tippe auf **[RAUM ERSTELLEN]**.

### Spieler einladen
* **QR-Code (Empfohlen):** Tippe als Host auf das kleine QR-Symbol (neben dem Raum-Code). Es öffnet sich ein QR-Code. Die Mitspieler scannen diesen mit ihrer Kamera, tragen ihren Namen ein und tippen auf **[RAUM BEITRETEN]**.
* **Manuell:** Gib den 4-stelligen Raum-Code an deine Mitspieler weiter. Diese geben ihn auf der Startseite unter "CODE" ein und tippen auf **[RAUM BEITRETEN]**.

### Offline-Spieler hinzufügen
Wenn jemand kein eigenes Smartphone nutzt:
1. Tippe auf **[+ Offline-Spieler]**.
2. Gib den Namen ein und tippe auf **[+]**.
*Diese Spieler erscheinen mit dem Zusatz "(kein Handy)" in der Liste. Der Host muss für diese Spieler den Zug manuell beenden.*

### Einstellungen
* **Reihenfolge:** Nutze die Pfeiltasten **[↑]** und **[↓]** neben einem Namen.
* **Spieler entfernen:** Tippe auf das rote **[X]**.
* **Audio-Steuerung:** Mit dem Lautsprecher-Symbol **[🔊 / 🔇]** legst du fest, welches Handy Ansagen/Töne wiedergibt.
* **Zeit einstellen:** Nutze den Schieberegler. *Tipp: Ein Doppelklick auf die Zeitangabe öffnet ein Eingabefeld für die punktgenaue Eingabe (z.B. "1.5" für 1:30 min).*

---

## 2. Während des Spiels

* **Zug beenden:** Wer am Zug ist, tippt auf **[WEITER]**.
* **Host-Kontrolle:** Der Host kann jederzeit über den Button **[NÄCHSTER: Name]** den Zug weitergeben, unabhängig davon, wer gerade aktiv ist.
* **Akustische Hinweise:** 
    * Halbzeit-Ansage (bei > 2 Min. Zugzeit).
    * "Noch 30 Sekunden" Warnung.
    * Countdown in den letzten 10 Sekunden (Piepsen + Ansage).
    * Zeit abgelaufen (2 Signaltöne).
* **Spielsteuerung:** Über **[ZUR LOBBY]** gelangst du zurück in die Einstellungen. **[SPIEL BEENDEN]** setzt den Timer zurück. 
* **Exit:** Über den **[EXIT]** Button oben rechts kannst du den Raum verlassen/schließen (mit Sicherheitsabfrage).

---

## 3. Technische Hinweise

**Direkte Verbindung (Peer-to-Peer)**
Sobald das Spiel läuft, tauschen eure Handys die Sekunden und Befehle direkt untereinander aus. Das sorgt für eine flüssige Steuerung ohne Verzögerung.

**Warum braucht man trotzdem Internet?**
Ihr benötigt eine aktive Internetverbindung, da das Internet als "Vermittler" dient:
1. **Verbindungsaufbau:** Es hilft den Handys, sich im Netzwerk zu finden.
2. **Automatischer Reconnect:** Wenn ein Handy durch den Standby-Modus die direkte Funkverbindung verliert, nutzt der Timer das Internet, um die Verbindung im Hintergrund blitzschnell und automatisch wiederherzustellen. Ohne diese Hilfe müsstet ihr nach jedem Standby den Raum neu betreten.
