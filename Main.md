# DataShield Datensicherungs lösung für unternehmen.

Ich möchte ein Produkt entwerfen bei dem man seine daten auf einem True nas server speichern kann und sich als client diese daten auch beziehen kann. Dann möchte ich es auch schaffen das es ein Backup des nas servers gib das an einem externen standort.

## Instalation TrueNas au HyerV-Manager
Ich habe mich für ein TrueNas als File server entschieden. Weil das für mich als die beste option erscheint da ich noch nicht damit gearbeitet habe und es so eine challenge für mich ist. Auch das es uns empfolen wurde und wir eine Anleitung für die installation erhalten haben hat mich dazu bewegt ein TrueNas zu verwenden. Jetzt zur installation. Ich habe meinem True nas 4 gb ram vergeben und eine Festplatte von 50gb. Eigentlich sind 8gb empfohlen jedoch brauche ich diese VM nur für testzwecke deshalt sollte dies reichen. Ich habe jetzt den server fertig aufgesetzt und kann per gui über den browser auf diesen server per GUI zugreifen.Ich habe eine statische ip adresse gesetzt damit ich leichter darauf zugreifen kann. Jetzt habe ich einen Linux server aufgesetzt und mit diesem Den nas server angeping und umgekehrt damit ich sicher sein kann das dass funktioniert mit der Verbindung.






Datensicherungskonzept

Datensicherheitskonzept:

Das Datensicherungssystem wird für die CRM Datenbank eines kleineren Betriebes konzipiert. Die Auslegung basiert auf den Empfehlungen der BSI CON.3 Datensicherungskonzept.

Auf Grund des Geschäftsmodell der Firma besteht keine regulatorische Pflicht die Daten länger aufzubewahren und es muss keine Archivierungslösung implementiert werden.

Rahmenbedingung für das Datensicherungskonzept.

Durch verschiedene Gespräche mit Businessvertretern wie auch den Fachverantwortlichen aus dem IT-Betrieb wurden folgende Rahmenbedingungen definiert:

• Speichervolumen:

o CRM Datenbankgrösse aktuell: 350GB

• Änderungsvolumen:

o Zunahme der CRM Datenbank war in der Vergangenheit ca. 10% /a

• Änderungszeitpunkte:

o Änderungszeitpunkt ist während den normalen Geschäftszeiten

o Der Backup wird nach Ende des Businesstages um 20Uhr gestartet.

• Verfügbarkeitsanforderungen:

o Der Geschäftsbetrieb könnte einen Tag ohne die Datenbank weitergeführt und nachgetragen werden

• Integritätsbedarf

o Der tägliche Integrity-Check der SQL Datenbank ist automatisiert und berichtet via Email

• rechtliche Anforderungen

o Es bestehen keine rechtliche Anforderungen oder Archivierungspflicht. Die üblichen GDPR Gesetze können über die CRM Applikation sichergestellt werden.

• Speichermedien

o 2 verschiedene NAS Speicher und eine wöchentliche Auslagerung in die Cloud

• Transportmodalitäten

o

• Aufbewahrungsmodalität

o Die Sicherungskopien werden 8 Tage zurück aufbewahrt und jeweils die letzte des Monats für 12 Monate.

• Datensicherungstests

o Der Status des täglichen Backups wird via Email informiert

o Können die Daten zurückgespielt werden

§ Monatlich wird ein Restore-Test durchgeführt initial werden die Restore-Tests wöchentlich (4mal) getestet und auch gleich als wiederholte Schulung