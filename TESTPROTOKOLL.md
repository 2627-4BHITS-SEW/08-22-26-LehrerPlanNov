Testdatum · 
Getesteter Commit · 

| Nr. | Durchführung | Soll | Ist | Status |
|---|---|---|---|---|
| 1 | | | | |

**5.11.2026** · …  
**88bcd09** · …

| Nr. | Durchführung | Soll | Ist | Status |
|---|---|---|---|---|
| 2 | Spiel gestartet. Die GameObjects `Sign-B310` und `Sign-C312` aufgesucht und die angezeigten Lehrkräfte notiert. Anschließend mit der Schulwebsite verglichen. | Jedes Schild zeigt seinen Raum und die zugehörigen Lehrkräfte. | Raumnummer und zugeordnete Personen stimmen auf beiden Schildern exakt mit den Daten der Website überein. Keine falschen Zuordnungen. | Bestanden |

Testdatum · 23.11.2026  
Getesteter Commit · `2c306ec`

| Nr. | Durchführung | Soll | Ist | Status |
|---|---|---|---|---|
| 3 | Direkt nach `await detailReq.SendWebRequest();` Raum, Lehrkraft, Detail-URL, HTTP-Status und Ergebnis per `Debug.Log`. Programm gestartet und in der Konsole nach der Detail-URL gesucht. | Für die passende Detailseite erscheint HTTP 200 (Success). | Für zB `https://www.htl-salzburg.ac.at/lehrerinnen-details/grossmaier-maria-rosa-prof-bed-univ-med-b-312.html` erscheint Raum B312, HTTP 200, Ergebnis Success. Auch die übrigen geloggten Detailseiten (z. B. B305, C312, B304) liefern HTTP 200 (Success). | Bestanden |

Testdatum · 
Getesteter Commit · 

| Nr. | Durchführung | Soll | Ist | Status |
|---|---|---|---|---|
| 4 | | | | |

Testdatum · 23.11.2026  
Getesteter Commit · `18988aa`

| Nr. | Durchführung | Soll | Ist | Status |
|---|---|---|---|---|
| 5 | In einer duplizierten Testszene ein neues Schild `B403` angelegt. Szene gestartet; die Übersicht wurde erfolgreich geladen. | Das Schild zeigt den Raumcode B403 und eine verständliche Meldung, dass keine Lehrkräfte gefunden wurden. | Am Schild erscheint nur „Lehrer im Raum B403:“ – keine Lehrkräfte und keine Meldung, dass keine gefunden wurden. | Fehlgeschlagen(Fixed) |

Testdatum · 
Getesteter Commit · 

| Nr. | Durchführung | Soll | Ist | Status |
|---|---|---|---|---|
| 6 | | | | |

Testdatum · 24.11.2026  
Getesteter Commit · `02a395f`

| Nr. | Durchführung | Soll | Ist | Status |
|---|---|---|---|---|
| 7 | Internetverbindung des Rechners getrennt (WLAN/LAN aus). Anwendung gestartet und gewartet, bis die Anfrage der Übersicht beendet ist. Ergebnis am Schild und `[Testfall 7]`-Log in der Console geprüft. | Am Schild steht „Fehler beim Laden der Lehrerliste!“. | Am Schild steht „Fehler beim Laden der Lehrerliste!“. | Bestanden |
