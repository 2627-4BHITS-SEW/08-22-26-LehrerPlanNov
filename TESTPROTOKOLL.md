Testdatum · 23.11.2026
Getesteter Commit · ee7fc36 (+ lokales Logging in `TextfieldScript.cs`, nicht committet)

| Nr. | Durchführung | Soll | Ist | Status |
|---|---|---|---|---|
| 1 | | | | |
| 2 | | | | |
| 3 | Direkt nach `await detailReq.SendWebRequest();` Raum, Lehrkraft, Detail-URL, HTTP-Status und Ergebnis per `Debug.Log`. Programm gestartet und in der Konsole nach der Detail-URL gesucht. | Für die passende Detailseite erscheint HTTP 200 (Success). | Für zB `https://www.htl-salzburg.ac.at/lehrerinnen-details/grossmaier-maria-rosa-prof-bed-univ-med-b-312.html` erscheint Raum B312, HTTP 200, Ergebnis Success. Auch die übrigen geloggten Detailseiten (z. B. B305, C312, B304) liefern HTTP 200 (Success). | Bestanden |
| 4 | | | | |
| 5 | In einer lokalen Testkopie der Szene ein Schildobjekt vor dem Start auf `Sign-A999` umbenannt (Raumcode ohne passenden Detail-Link in der Übersicht). Szene gestartet und über das `[Testfall 5]`-Log geprüft, dass die Übersicht erfolgreich geladen wurde (HTTP 200, Success). | Das Schild zeigt den Raumcode A999 und eine verständliche Meldung, dass keine Lehrkräfte gefunden wurden. | _TODO_ | _TODO_ |
| 6 | | | | |
| 7 | | | | |