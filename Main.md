# DataShield Datensicherungs lösung für unternehmen.

Ich möchte ein Produkt entwerfen bei dem man seine daten auf einem True nas server speichern kann und sich als client diese daten auch beziehen kann. Dann möchte ich es auch schaffen das es ein Backup des nas servers gib das an einem externen standort.

## Instalation TrueNas au HyerV-Manager
Ich habe mich für ein TrueNas als File server entschieden. Weil das für mich als die beste option erscheint da ich noch nicht damit gearbeitet habe und es so eine challenge für mich ist. Auch das es uns empfolen wurde und wir eine Anleitung für die installation erhalten haben hat mich dazu bewegt ein TrueNas zu verwenden. Jetzt zur installation. Ich habe meinem True nas 4 gb ram vergeben und eine Festplatte von 50gb. Eigentlich sind 8gb empfohlen jedoch brauche ich diese VM nur für testzwecke deshalt sollte dies reichen. Ich habe jetzt den server fertig aufgesetzt und kann per gui über den browser auf diesen server per GUI zugreifen.Ich habe eine statische ip adresse gesetzt damit ich leichter darauf zugreifen kann. Jetzt habe ich einen Linux server aufgesetzt und mit diesem Den nas server angeping und umgekehrt damit ich sicher sein kann das dass funktioniert mit der Verbindung.






Datensicherungskonzept

Datensicherheitskonzept:

Das Datensicherungssystem wird für die CRM Datenbank eines kleineren Elektrikrer-Betriebes konzipiert. Die Auslegung basiert auf den Empfehlungen der BSI CON.3 Datensicherungskonzept.

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



## Tagesrefelxion

27.10.2023

Ich habe heute mit Herr Rohr über mein Datensicherungskonzept gesprochen. Wir haben es analysiert und ich bin auf dem Guten weg ich müsste Jedoch noch das GeBüv beachten das habe ich heute noch nicht getan. Ich habe jedoch mein TrueNas erfolgreich neu afgesetzt das es mir am Anfang nicht möglich war einen Datenpool zu erstellen da es beim HyperV manager nicht möglich ist eine zusätzliche Festplatte mitzugeben beim erstellen einer VM. Oder ich habe einfach nicht herausgefunden wie. Jedoch habe ich dan nochmals die Einstellungen analysiert und herausgefunden das man nachträglich eine Zusätzliche Fesplatte hinzufügen kann. Das habe ich heute erreicht und habe es die dletzten Wochen for mir hergeschoben da ich dachte das wäre mit dem HyperV nicht möglich ich jedoch auch nicht die applikation zum starten der Vms wechseln wollte da ich mit HyperV sehr gute Erfahrungen gemacht habe.

Ich bin vorallem mit der Planung weiter gekommen da ich mir jetzt mein Endprodukt konkret vorstellen kann. Ich habe auch schon im kopf wie ich es umsetzten werde jedoch gibt es noch ein paar Schen die mir noch unklar sind wie ich sie Lösen werde. Ich habe die Aufgabe verschoben mir zu überlegen wie ich eine Datenbank erstelle die ich nacher BAckupen will jedoch habe ich schon die Verbindungen zwischen den verschiedenen Clients überprüft und die funktioniert. Ein unnötiger Zeitfreeser war das ich als mein NAS Korrupt war oder einfach nicht mer funktioniert hatt das ich versucht habe das zu reparieren ob wohl ich auf diesem NAS sonst noch nichts gemacht habe und es 100 mal schneller gewesen wäre war es einfach neu aufzusetzten.




