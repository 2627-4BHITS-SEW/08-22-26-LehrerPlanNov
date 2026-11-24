Testdatum · 23.11.2026
Getesteter Commit · ee7fc36 (+ lokales Logging in `TextfieldScript.cs`, nicht committet)

| Nr. | Durchführung | Soll | Ist | Status |
|---|---|---|---|---|
| 1 | | | | |
| 2 | | | | |
| 3 | Direkt nach `await detailReq.SendWebRequest();` Raum, Lehrkraft, Detail-URL, HTTP-Status und Ergebnis per `Debug.Log`. Programm gestartet und in der Konsole nach der Detail-URL gesucht. | Für die passende Detailseite erscheint HTTP 200 (Success). | Für zB `https://www.htl-salzburg.ac.at/lehrerinnen-details/grossmaier-maria-rosa-prof-bed-univ-med-b-312.html` erscheint Raum B312, HTTP 200, Ergebnis Success. Auch die übrigen geloggten Detailseiten (z. B. B305, C312, B304) liefern HTTP 200 (Success). | Bestanden |
| 4 | | | | |
| 5 | In einer duplizierten Testszene ein neues Schild `B403` angelegt. Szene gestartet; die Übersicht wurde erfolgreich geladen. | Das Schild zeigt den Raumcode B403 und eine verständliche Meldung, dass keine Lehrkräfte gefunden wurden. | Am Schild erscheint nur „Lehrer im Raum B403:“ – keine Lehrkräfte und keine Meldung, dass keine gefunden wurden. | Fehlgeschlagen(Fixed) |
| 6 | | | | |
| 7 | Internetverbindung des Rechners getrennt (WLAN/LAN aus). Anwendung gestartet und gewartet, bis die Anfrage der Übersicht beendet ist. Ergebnis am Schild und `[Testfall 7]`-Log in der Console geprüft. | Am Schild steht „Fehler beim Laden der Lehrerliste!“. | Am Schild steht „Fehler beim Laden der Lehrerliste!“. | Bestanden |