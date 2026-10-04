# Datenschutzrichtlinie für GeoSweeper

**Datum des Inkrafttretens:** 26. September 2026

**Letzte Aktualisierung:** 4. Oktober 2026

## Die Kurzversion

GeoSweeper erhebt, überträgt, verkauft oder teilt keinerlei personenbezogene Daten. Jedes Brett, das Sie spielen, jede Einstellung, die Sie auswählen, und jedes Land, das Sie gemeistert haben, wird nur auf Ihrem Gerät gespeichert. Es wird nichts bei uns hochgeladen und es muss überhaupt kein Konto erstellt werden. Der einzige Netzwerkverkehr, den GeoSweeper jemals generiert, ist StoreKit, der mit Apple kommuniziert, wenn Sie einen Kauf tätigen oder wiederherstellen, und Seiten, die Sie absichtlich über einen Link innerhalb der App öffnen (diese Website oder Apples eigene rechtliche Seiten) – beide werden im Folgenden behandelt und keines von beiden enthält etwas anderes.

## Wer wir sind

GeoSweeper wurde von Ivan Cayabyab entwickelt. Fragen zu dieser Richtlinie oder zur App können an ivnsjdev@gmail.com gesendet werden.

## Was die App speichert und wo

Alles unten befindet sich nur auf Ihrem Gerät, an einem von drei Orten: „UserDefaults“ (kleine Einstellungswerte), einer JSON-Datei im eigenen Application Support-Ordner der App oder einer lokalen SQLite-Datenbank.

| Was | Primärspeicher | Automatisch an uns gesendet? |
|---|---|---|
| Display settings — board theme, neon color, explosion effect, blast sound, map projection (globe or flat), sound and haptics on/off | `UserDefaults` | Nein |
| Language, das Sie in der App ausgewählt haben | `UserDefaults` | Nein |
| Verwaltung der Bewertungsanfrage – die Daten, an denen GeoSweeper iOS gebeten hat, die native Bewertungsabfrage anzuzeigen, und welcher Meilenstein die letzte ausgelöst hat | `UserDefaults` | Nein |
| Zähler für Gratisspiele – wie viele Ihrer 10 kostenlosen Kartenländer und Ihrer 10 kostenlosen **Classic**-Spiele Sie verbraucht haben | `UserDefaults` | Nein |
| Rekord pro Land – Siege, Niederlagen, Bestzeit und wann Sie ihn freigeschaltet haben, für jedes Land, in dem Sie gespielt haben | A JSON file (`progress.json`) in the app's Application Support folder | Nein |
| **Classic**-Verlauf – die Brettgröße, der Schwierigkeitsgrad, die Anzahl der Minen, die Zeit und Sieg oder Niederlage jedes abgeschlossenen Classic-Spiels | Eine JSON-Datei (`Classic/history.json`) im Application Support-Ordner der App | Nein |
| Infinite Tower Fortschritt – die Zeile, die Sie erreicht haben, Ihr gespeichertes Ansichtsfenster und welche Zeilen Sie gelöscht haben | Eine lokale SQLite-Datenbank | Nein |

Nichts davon wird an Dritte weitergegeben oder verkauft, auch nicht an uns. Der eigene Datenverkehr von StoreKit (siehe unten) und die externen Links, auf die Sie tippen (ebenfalls unten), übertragen nichts davon. Eine iOS-Gerätesicherung kann diese Dateien als Teil der Sicherung der App als Ganzes enthalten – diese Sicherung wird von Ihnen oder von iOS initiiert, niemals von GeoSweeper, und sie verbleibt dort, wo Sie sie senden (iCloud oder Ihr Computer), nicht bei uns.

## Kein Konto, keine Anmeldung, keine Cloud

GeoSweeper fragt niemals nach einem Namen, einer E-Mail-Adresse, einer Telefonnummer, einem Geburtsdatum oder anderen identifizierenden Informationen – es gibt nichts, mit dem man sich anmelden kann, da kein Konto vorhanden ist. Ihr Fortschritt wird weder über iCloud, CloudKit noch über einen anderen Dienst synchronisiert: Er existiert nur auf dem Gerät, auf dem Sie spielen. Spielen Sie dasselbe Land auf einem zweiten Gerät und es beginnt dort von vorne, da es nirgendwo eine Serverkopie gibt, von der aus synchronisiert werden kann.

## Alles wurde absichtlich nicht beharrt

Das Spielfeld, auf dem Sie sich befinden – jedes geöffnete Plättchen, jede platzierte Flagge – wird nur im Arbeitsspeicher gehalten, während Sie spielen. Das gilt in allen drei Welten: der Karte, dem **Classic**-Modus und **Infinite Tower**. Wenn Sie die App mitten im Spiel schließen, ist das Spielbrett verschwunden. Es wird nie auf die Festplatte geschrieben und es gibt keine automatische Speicherung, um ein unvollendetes Board fortzusetzen. Nur ein *abgeschlossenes* Spiel (ein Sieg oder eine Niederlage) aktualisiert den oben beschriebenen Länderrekord oder den Classic-Verlauf.

## Das Einzige, was sich anhört, als wäre es nicht lokal

Beim ersten Start der App wird die Karte für Ihr eigenes Land geöffnet. Dies kommt von der **Regionseinstellung** Ihres Geräts (das Land, das an Ihre Sprache und Ihr Gebietsschema gebunden ist, dasselbe, das iOS verwendet, um eine Tastatur und einen Kalender auszuwählen) – nicht von GPS, WLAN oder einer anderen Form der Standortverfolgung. GeoSweeper fordert keinen Standortzugriff an und könnte Ihre Koordinaten selbst dann nicht auslesen, wenn es wollte.

## Berechtigungen

GeoSweeper fordert überhaupt keine Systemberechtigungen an. Es wird niemals nach der Kamera, der Fotobibliothek, dem Mikrofon, dem Standort, den Kontakten, dem Kalender, den Gesundheitsdaten, den Bewegungsdaten oder den Push-Benachrichtigungen gefragt, und es wird niemals eine Erlaubnisanfrage jeglicher Art angezeigt. Dies entspricht genau der „Info.plist“ der App: Es gibt keinen einzigen Nutzungsbeschreibungseintrag darin.

## Einkäufe

GeoSweeper kann kostenlos heruntergeladen werden, und jede seiner drei Welten hat ihre eigene kostenlose Testversion. Ihre ersten 10 Länder auf der Karte – jede Stufe, einschließlich Beginner – können kostenlos gespielt werden, und sobald Sie ein Land gespielt haben, bleibt es dauerhaft wiederspielbar, auch nach Ablauf dieser Testversion. Der **Classic**-Modus gibt Ihnen auf dieselbe Weise 10 kostenlose Spiele. Infinite Tower ist bis Zeile 10 kostenlos. Über diese Punkte hinaus gibt es drei unabhängige Käufe, alle einmalig, nicht verbrauchbar, über Apples StoreKit angeboten und vollständig von Apple abgewickelt:

- **All Countries** – ein einmaliger, nicht verbrauchbarer Kauf, der die Stufen Intermediate, Expert und Mega in allen 204 Ländern dauerhaft freischaltet. Daran ändert sich nichts.
- **Classic Lifetime** – ein einmaliger, nicht verbrauchbarer Kauf, der unbegrenzte Classic-Spiele dauerhaft freischaltet, sobald Ihre 10 kostenlosen aufgebraucht sind. Daran ändert sich nichts.
- **Infinite Tower Lifetime** – ein einmaliger, nicht verbrauchbarer Kauf, der das Weiterklettern über Zeile 10 hinaus dauerhaft freischaltet. Auch das wird nicht verlängert, und GeoSweeper bietet keinerlei Abonnement an.

Apple, nicht GeoSweeper, verarbeitet jede Zahlung. Keine Kartennummer, Rechnungsadresse oder Apple Account-Anmeldeinformation ist für uns jemals sichtbar – StoreKit teilt der App nur mit, was sie benötigt, um eine Paywall anzuzeigen und Zugriff zu gewähren: den anzuzeigenden Preis und ob Sie derzeit jeden Artikel besitzen. Diese Antworten bleiben auf Ihrem Gerät; GeoSweeper betreibt keinen eigenen Kaufserver und kann sie nirgendwohin senden. Bei der Wiederherstellung von Einkäufen wird Apple aufgefordert, den Besitz Ihres Apple Account erneut zu bestätigen, und die Antwort wird lokal angewendet – es werden keine neuen Datensätze erstellt oder übertragen.

Siehe auch Apples [App Store & Privacy](https://www.apple.com/legal/privacy/data/en/appstore/), die [Apple Media Services Terms and Conditions](https://www.apple.com/legal/internet-services/itunes/) und die [Standard End User License Agreement](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/), die den Kauf selbst regeln.

## Unterstützen Sie die Kommunikation

Wenn Sie eine E-Mail an ivnsjdev@gmail.com senden, erhalten wir Ihre E-Mail-Adresse, alles, was Sie schreiben, und jeden Anhang, den Sie hinzufügen. Wir verwenden diese Daten nur, um Ihnen zu antworten und das Problem zu beheben, über das Sie geschrieben haben. Unsere Rechtsgrundlage ist unser berechtigtes Interesse, den Personen zu antworten, die uns kontaktieren. Bei diesem Postfach handelt es sich um ein Standard-Gmail-Konto, das von Google LLC gemäß [der Datenschutzrichtlinie von Google](https://policies.google.com/privacy) verarbeitet und auf einer Infrastruktur gehostet wird, die sich möglicherweise außerhalb Ihres eigenen Landes befindet, weshalb diese Übertragung hier offengelegt wird. Wir bewahren Support-E-Mails bis zu 24 Monate lang auf und löschen sie dann; Sie können uns jederzeit bitten, eine bestimmte E-Mail früher zu löschen, indem Sie an dieselbe Adresse schreiben.

## Externe Links

Die Paywalls von GeoSweeper verweisen auf die Datenschutzrichtlinie dieser Website und auf die Standard-EULA von Apple. Settings kann auf die Seite „Rezension schreiben“ des App Store verlinken. An keinem dieser Links werden Benutzerdaten oder App-spezifische Kennungen angehängt – es handelt sich um einfache URLs, die für alle gleich sind.

## Nichts zu wetten

GeoSweeper has no in-app currency, no loot, no prize draws, and no feature where an outcome is staked or wagered. Bei jedem Kauf handelt es sich um einen festen, offengelegten Preis für den dauerhaften oder zeitlich begrenzten Zugriff auf Inhalte; Es kann nichts gewonnen, verloren oder verspielt werden.

## Was wir NICHT tun

- Keine Analysen, Absturzberichte oder Telemetrie jeglicher Art
- Keine Werbung, keine Werbenetzwerke und keine Werbekennungen
- Kein App- oder Site-übergreifendes Tracking und keine Datenbroker
- Keine Konten, keine Anmeldung, keine Passwörter
- Keine Kamera, Fotobibliothek, Mikrofon, Kontakte, genauer oder grober Standort oder Gesundheitsdaten
- Kein Training von maschinellen Lernmodellen auf Ihren Daten
- Keine SDKs jeglicher Art von Drittanbietern – der einzige Code in dieser App ist unser eigener

Dies entspricht dem Etikett „Data Not Collected (keine Daten erfasst)“, das GeoSweeper auf dem App Store trägt.

## Aufbewahrung und Löschung

Durch das Löschen der App werden alle auf Ihrem Gerät gespeicherten Dateien – Einstellungen, Ihr länderspezifischer Datensatz, Ihr Classic-Verlauf und Ihr Infinite Tower-Fortschritt – sofort und vollständig gelöscht, da es nie eine Serverkopie gab, die wir behalten oder löschen konnten. An iCloud device backup made before deletion may still contain a copy; Dieses Backup unterliegt vollständig Ihrer Kontrolle über **Settings → Ihr Name → iCloud → Kontospeicher verwalten** auf Ihrem Gerät. Support-E-Mails werden wie oben beschrieben separat aufbewahrt und gelöscht.

## Ihre Rechte

Da GeoSweeper keine Kopie Ihrer In-App-Daten speichert, sind die Zugriffs-, Korrektur-, Export- und Löschrechte gemäß DSGVO, UK DSGVO und CCPA/CPRA diejenigen, die Sie bereits direkt auf Ihrem eigenen Gerät ausüben – es gibt hier keine Aufzeichnungen, die wir in Ihrem Namen erstellen oder löschen könnten. Der einzige Ort, an dem wir etwas aufbewahren, ist eine Support-E-Mail, die Sie uns gesendet haben. Sie können diese jederzeit einsehen, korrigieren oder löschen lassen, indem Sie an ivnsjdev@gmail.com schreiben. Wir verkaufen oder teilen keine personenbezogenen Daten für kontextübergreifende Verhaltenswerbung und haben dies auch nie getan. Wenn Sie glauben, dass wir mit Ihren Daten falsch umgegangen sind, haben Sie das Recht, eine Beschwerde bei Ihrer örtlichen Datenschutzbehörde einzureichen.

## Kinder

GeoSweeper verfügt über eine Altersfreigabe, die für ein allgemeines Publikum geeignet ist, und richtet sich nicht speziell an Kinder. Wir sammeln wissentlich keine personenbezogenen Daten von irgendjemandem, auch nicht von Kindern unter 13 Jahren, und es gibt nichts in der App, das dies könnte – kein Chat, kein Teilen, keine soziale Funktion, keine Werbung und kein Konto, über das Dritte ein Kind erreichen könnten.

## Änderungen an dieser Richtlinie

Wenn sich diese Richtlinie ändert, ändert sich auch das Datum oben, und eine wesentliche Änderung an dem, was GeoSweeper mit Daten macht, wird auch in den Versionshinweisen zu diesem Update vermerkt.

## Kontakt

ivnsjdev@gmail.com
