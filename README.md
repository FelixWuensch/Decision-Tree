# Decision-Tree
Prüfungsaufgabe 1 - Zweiter Teil

Um dieses Projekt zu starten, folgen Sie dem Binder Badge:      [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/FelixWuensch/Decision-Tree/main)

# Ausführung der Übungsaufgabe

!!! Alle Befehle werden ausgeführt in dem die Zeile ausgewählt wird und anschließend mit Shift (Großschreibtaste) und Enter gestartet wird !!!

1. Im ersten Schritt müssen alle benötigten Libraries installiert und importiert werden, so dass im Folgenden alle Befehle erfolgreich ausgeführt werden können.
2. Danach werden unsere Daten im CSV Format eingelesen.
3. Daraufhin werden die Daten wieder begutachtet mit den üblichen drei Funktionen: .info(), .descrive(), .head().
4. Dann gehen wir über und starten mit der explorativen Datenanalyse. Dafür legen wir zunächst zwei Histogramme übereinander und lassen uns die Spalte „fico“ anzeigen, aufgeteilt nach „credit.policy“ gleich null und eins. Das nächste Diagramm ist dasselbe noch einmal nur dieses Mal betrachten wir statt „credit.policy“ die Spalte „not.fully.paid“.
5. Im fünften Schritt wird ein Countplot erstellt, welches die Spalte „not.fully.paid“ aufschlüsselt anhand der „purpose“ (X-Ache) Spalte. Daraufhin erstellen wir ein Jointplot mit den Daten „fico“ (X-Achse) und der „int.rate“ (Y-Achse). Durch das Jointplot lässt sich der Trend zwischen „fico“ und der „int.rate“ beschreiben.
6. Beim nächsten Diagramm handelt es sich um zwei Lmplots. Hierbei untersuchen wir wie sich der Trend zwischen der Spalte „not.fully.paid“ und der Spalte „credit.policy“ verhält und können ablesen wie dieser sich unterscheidet. 
7. Dann werden auch schon die Daten vorbereitet. Dazu schauen wir sie uns noch mal an mit .info(). Dann müssen wir Dummy-Variablen für die Spalte „purpouse einfügen, da diese zuvor mit Objekten gefüllt war, welche von den Entscheidungsbäumen verwendet werden kann.
8. Nach dem die Dummy-Varialben erfolgreich eingefügt wurden, können wir nun dazu übergehen die Daten aufzuteilen in die Trainings- und Testdaten.
9. Nun wird die Klasse für die Decision Trees importiert, ein Decision Tree angelegt und auch direkt mit den Trainingsdaten trainiert.
10. Im Anschluss wird eine Vorhersage durch das Trainierte Modell generiert. Diese Vorhersage wollen wir auch direkt wieder Anschauen in dem wir die Classification Report und die Confusion Matrix importieren und uns ausgeben lassen 
11. Jetzt machen wir das ganze noch einmal, jedoch mit einem Random Forest Modell. Dieses wird dafür importiert, angelegt und auch direkt mit den Trainingsdaten trainiert.
12. Auf den Randoom Forest Tree wird dann auch wieder eine Vorhersage generiert. Diese wird erneut mit dem Classification Report und der Confusion Matrix begutachtet.
13. Wir haben beide Tree Arten angelegt, damit wir diese auch vergleichen können. Beide liefern Ergebnisse, jedoch sind die Ergebnisse nicht perfekt. Man müsste beide Arten weiter optimieren um ein bessere Ergebnisse erzielen zu können. Dies erreicht man in dem man die Eigenschaften der Bäume anpasst. 


Damit ist das Kapitel der Entscheidungsbäume abgeschlossen. Wir haben uns dafür die Daten genauer angeschaut mit der explorativen Datenanalyse um eine gute Aufteilung der Daten treffen zu können. Dann haben wir die Aufteilung vorgenommen, die Modele erstellt, trainiert und eine Vorhersage treffen lassen. Zu guter Letzt haben wir die Vorhersagen auf seine Genauigkeit untersucht und beide Arten von Entscheidungsbäumen miteinander verglichen. Somit gehen wir weiter zum Thema K Means Clustering.

