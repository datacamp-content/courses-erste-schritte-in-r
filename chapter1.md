---
title: 'Erste Schritte für einen interaktiven Beginn für R Starter und Data Science Neulinge'
description: 'Mit diesem kurzen, anschaulichen Einstieg erhalten Sie einen leichten Einstieg in die Programmiersprache R. Er eignet sich für eine schnelle Auffrischung oder für Neulinge - fangt einfach an! Viel Spaß dabei.'
free_preview: true
---

## Wie R in DataCamp funktioniert

```yaml
type: NormalExercise
key: 6321c28123
xp: 100
```

Hauptfunktionen:

Linke Funktionsseite:
- 1) Hier im **Exercisebereich** wird immer die grundlegende Theorie dargestellt sein, die dann direkt in der Übung angewendet wird. 
- 2) Im Bereich der **Instruktion** bekommen Sie die Erläuterung, was genau Ihre Aufgabe ist, die Sie anschließend lösen sollen. 
- 3) Die **Hints** können Sie nutzen, wenn Sie nicht mehr weiter kommen und einen Hinweis benötigen.

rechte Funktionsseite:
- 4) **script.R** ist ihre Kommandozeile mit der Sie Ihre Befehle und Ihren Code in der Programmiersprache R eingeben.
- 5) Mithilfe des Buttons **Run Code** kompilieren Sie nur den Code mit **Submit Answer** führen Sie ihn aus.
- 6) Die **Console** ist in diesem Fall eine Oberfläche in der Sie sehen können, wie Ihr geschriebener Code ausgeführt wird und welche Ausgaben er liefert.

`@instructions`
Hallo und herzlich Willkommen,

Sie sind unser/e neue/r MitarbeiterIn in der **Abteilung Business Intelligence & Data Analytics** und befassen sich das erste Mal mit der Programmiersprache R. Ihr Chef Herr Müller hat Ihnen verschiedene Aufgaben gegeben - nun fangen wir aber erstmal leicht an. 

- Wir fangen mit dem Programm an mit dem fast alle Programmierbücher starten:
	- Dafür schreiben Sie bitte: **print("Hello World!")** in das Skript und drücken auf 'Submit Answer'.

`@hint`
Keine Angst - einfach print("Hello World!") in das Skript schreiben und auf 'Submit Answer' drücken.

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}
# Ihr erstes Programm: "Hello World!"

```

`@solution`
```{r}
# Ihr erstes Programm: "Hello World!"
print("Hello World!")
```

`@sct`
```{r}
ex() %>% check_output("Hello World!", fixed=TRUE, missing_msg= "So ist das nicht ganz richtig - Beachten Sie Tippfehler!")
success_msg("So ihr erstes Programm ist vollendet!")
```

---

## Rechnen in R

```yaml
type: TabExercise
key: 3fe708c52e
xp: 100
```

R kann in seiner Basisfunktion als Rechner verwendet werden. Beachten Sie folgende arithmetische Rechenoperatoren:	 

```
 Addition: + 
 Subtraktion: - 
 Multiplikation: *
 Division: / 
 Potenzierung: ^
 Modulo: %%
```
 
Der Operator Modulo (%%) liefert den Rest der Division der linken Zahl durch die rechte Zahl. Z.B.: 7 %% 2 ist 1.

Behalten Sie diese Informationen im Hinterkopf und befolgen Sie sie in den nachfolgenden Aufgaben, um die Übung erfolgreich abzuschließen.

`@pre_exercise_code`
```{r}

```

***

```yaml
type: NormalExercise
key: 92cdd27ee5
xp: 25
```

`@instructions`
- 1) Sie sollen die Umsätze der letzten drei Monate zusammenrechnen und somit den Umsatz für das Quartal Q1 erstellen. Fügen Sie bitte eine weitere Codezeile, die Rechnung, hinzu und klicken Sie danach auf "Submit Answer".

- Umsatz in €: Jannuar 234000 | Februar 320000 | März 294000

`@hint`
Stellen Sie sicher, dass Sie die Summe aus 234000 + 320000 + 294000 in einer neuen Zeile eingefügt haben. Starten Sie die Zeile nicht mit einem '#'-Zeichen, ansonsten wird der geschriebene Code nicht wie gewünscht ausgeführt, da damit Kommentare gekennzeichnet werden!

`@sample_code`
```{r}
# Beispielcode Addition 
67+78
# Quartalsumsatz Q1:

```

`@solution`
```{r}
# Beispielcode Addition 
67+78
# Quartalsumsatz Q1:
234000 + 320000 + 294000
```

`@sct`
```{r}
ex() %>% check_output(848000, fixed=TRUE, missing_msg="Sie müssen sich verrechnet haben. Beachten Sie auch mögliche Tippfehler!")
success_msg("Ja, genau - der Umsatz im ersten Quartal beträgt 848000€!")
```

***

```yaml
type: NormalExercise
key: aa4dc628ea
xp: 25
```

`@instructions`
- 2. Sie hatten im Quartal Q1 einen Umsatz von 848000€ zuerst ausgegeben. Aufgrund eines Forderungsausfalles von 42800€ müssen diese am Umsatz berücksichtigt werden.

`@hint`
Hier müssen Sie nur zwei Werte voneinander substrahieren.

`@sample_code`
```{r}
# Rückstellung berücksichtigen

```

`@solution`
```{r}

848000-42800
```

`@sct`
```{r}
ex() %>% check_output(805200, fixed=TRUE, missing_msg= "So ist das nicht richtig - beachten Sie Tippfehler!")
success_msg("Richtig! Wir haben nun einen Umsatz in Q1 von 805200€")
```

***

```yaml
type: NormalExercise
key: d41c199018
xp: 25
```

`@instructions`
- 3. Es sind auf den Umsatz von 295005€ im Januar eine Umsatzsteuer in Höhe von 56050.95€ aufgeschlagen worden. Wie viel Prozent an Umsatzsteuer wurden zur späteren Weitergabe an den Verbraucher aufgeschlagen, wenn die gesamte Steuer weitergegeben wurde? Geben Sie bitte das **Ergebnis in Prozent** aus!

`@hint`
Schauen Sie nochmal konkret auf Ihre Berechnung und überlegen Sie sich, wie Sie eine Verhältnisgleichung aufstellen. Es kann Ihnen helfen, an den Dreisatz aus Ihrer Schulzeit zu denken. Beachten Sie, dass in R anstatt dem Komma als Dezimaltrennzeichen der Punkt verwendet wird!

`@sample_code`
```{r}
# Ausrechnen der Umsatzsteuer

```

`@solution`
```{r}
56050.95/(295005/100)
```

`@sct`
```{r}
ex() %>% check_output("19", fixed=TRUE, missing_msg="Nicht ganz richtig - beachten Sie Tippfehler!")
success_msg("Richtig und die nächste Aufgabe!")
```

***

```yaml
type: NormalExercise
key: 1664766f3d
xp: 25
```

`@instructions`
- 4. Die Umsätze sollen in Q2 um 2.2% im Monat steigen. Welche Prognose geben Sie für die Umsatzzahlen am Ende des Q2 ab? Nehmen Sie den  Ausgangswert von 805200€ am Ende von Q1 an.

`@hint`
Beachten Sie, dass die Prozente jeweils im Monat steigen. Beachten Sie, dass in R anstatt dem Komma als Dezimaltrennzeichen der Punkt verwendet wird!

`@sample_code`
```{r}
# Umsatzprognose Q2

```

`@solution`
```{r}

805200*(1.022^3)
```

`@sct`
```{r}
ex() %>% check_output(859520.9, fixed=TRUE, missing_msg="So ist das nicht ganz richtig - haben Sie den monatlichen Umsatzwachstum berechnet und beachtet, dass es sich um 3 Monate handelt?!")
success_msg("Richtig und die nächste Aufgabe!")
```

---

## Variablen

```yaml
type: NormalExercise
key: 9ba097814a
xp: 100
```

Variablen zuweisen und vergleichen:

Ein grundlegendes Konzept in der (statistischen) Programmierung sind Variablen. Eine Variable ermöglicht es einen Wert (z.B. 5) oder eine Zeichenkette (z.B. "Funktionsbeschreibung") in R zu speichern. Später können Sie den Namen der Variable nutzen, um einfach auf den Wert oder das Objekt zuzugreifen, die innerhalb dieser Variablen hinterlegt sind (de Vries/ Meys 2018, S.45 & 86).
- Beispiel: So können Sie der Variable my_var den Wert 5 zuweisen: **my_var <- 5**

```
Variablen vergleichen:
x == y 		TRUE, wenn x exakt mit y übereinstimmt
x != y 		TRUE, wenn x von y abweicht
x > y  
x >= y
x & y 		x logisch-und y
x | y  		x logisch-oder y
!x    		nicht x
xor(x, y) 	exklusiv x logisch-oder y

```

`@instructions`
Herr Müller bittet Sie sich mit den Quartalszahlen der letzten und aktuellen Quartale vertraut zu machen.

1. Sie sollen nun die Quartalszahlen 2019 aus Q1: 805200€  und Q2: 859520.9€ den Variablen x und y zuordnen, um besser die Werte vergleichen zu können. 
2. In der Variable z wurden die Quartalszahlen aus Q3 & Q4 bereits hinterlegt und zugewiesen. Ist es richtig, dass das letzte Halbjahr 2018 erfolgreicher war als das Halbjahr 2019 sich zu entwickeln scheint, wie Herr Müller vermutet?

`@hint`
Schauen Sie bitte in die Exercisebox. Hier ist die Zuweisung anhand eines Beispiels verdeutlicht. Lesen Sie bitte genau die Instruktionen. Der Wert für Variable z wurde bereits zugewiesen.

`@pre_exercise_code`
```{r}
z <- 1655000
```

`@sample_code`
```{r}
# 1.Q1:

# Q2

# 2.Vergleich der halbjährlichen Umsätze aus 2018 und 2019: 

```

`@solution`
```{r}
# Q1
x <- 805200
# Q2
y <- 859520.9
# 2.Vergleich der Umsätze
z > (x+y)
```

`@sct`
```{r}
ex() %>% check_object("x") %>% check_equal(805200)
ex() %>% check_object("y") %>% check_equal(859520.9)
ex() %>% check_output("FALSE", fixed=TRUE, missing_msg= "Da haben Sie etwas falsch verglichen bei Aufgabe 2 oder die Aussage von Herrn Müller nicht direkt überprüft!")
success_msg("Ja, genau - es sieht so aus als hätten Sie die Variablenzuweisung verstanden und Herr Müller lag mit seiner Prognose falsch. Deshalb ist eine Überpüfung anhand von Daten für fundierte Aussagen und unternehmensrelevante Entscheidungen immer notwendig und wird in Zukunft weiter an Bedeutung zunehmen!")
```

---

## Datentypen in R

```yaml
type: TabExercise
key: 593549bc37
xp: 100
```

R arbeitet mit zahlreichen Datentypen und ist sensitiv auf Groß-/Kleinschreibung. Einige der grundlegendsten Datentypen sind:

![Datentypen](https://assets.datacamp.com/production/repositories/5050/datasets/9b03e35de433daa0c560843afc3955d82c6b6928/Basisdatentypen_%C3%9Cbersicht.PNG)

**Wichtig:** Zeichenketten werden in "Anführungszeichen" gesetzt.

Von einer kleinen Tochtergesellschaft hat Ihr Chef Herr Müller einen Kundendatensatz zugeschickt bekommen. Er sagt Ihnen, dass die Mitarbeiter dort noch nicht vertraut mit den Datentypen seien. Deswegen müssen Sie sich damit beschäftigen, um dies zu überprüfen.

`@pre_exercise_code`
```{r}
Anzahl_Mitarbeiter <- "Schmidt, Klaus"
```

***

```yaml
type: NormalExercise
key: 06523db4c2
xp: 35
```

`@instructions`
- 1. Die Variable **Anzahl_Mitarbeiter** müsste ein numerischer Basisdatentyp sein. Überprüfen Sie dies bitte.

`@hint`
Schreiben Sie bitte den Code so, damit als Output ein boolescher Wert (TRUE oder FALSE) ausgegeben wird! Schauen Sie in die Tabelle unter **Abfrage (Query)**

`@sample_code`
```{r}
#1.Überprüfung Datentyp Variable Anzahl_Mitarbeiter:

```

`@solution`
```{r}
#1.Überprüfung Variable Anzahl_Mitarbeiter:
is.numeric(Anzahl_Mitarbeiter)
```

`@sct`
```{r}
ex() %>% check_output(c(FALSE, "character"), fixed=TRUE, missing_msg= "Nicht richtig. Schreiben Sie bitte den Code so, damit als Output ein boolescher Wert ausgegeben wird!")
success_msg("Super, es ist keine numerische Variable hinterlegt, da müssen die Mitarbeiter der Tochtergesellschaft etwas falsch zugewiesen haben!")
```

***

```yaml
type: NormalExercise
key: 1aac779396
xp: 35
```

`@instructions`
- 2. Lassen Sie sich bitte die Variable **Anzahl_Mitarbeiter** ausgeben und wenn nicht die Anzahl von **17** hinterlegt ist, tun Sie dies bitte. Klicken Sie zur Zwischenausgabe auf 'Run Code'.

`@hint`
Eine Zuweisung (<-) funktioniert mit diesem Zeichen in R. Weisen Sie der Variablen den numerischen Wert 17 zu.

`@sample_code`
```{r}
#1.numerische Variable?
is.numeric(Anzahl_Mitarbeiter)
#Den Befehl class(Anzahl_Mitarbeiter) können Sie auch verwenden. Er gibt direkt den Basisdatentyp aus.
#2.Ausgabe + Zuweisung


```

`@solution`
```{r}
#2.1 Ausgabe und ggf. neue Zuweisung
print(Anzahl_Mitarbeiter)
#Den Befehl class(Anzahl_Mitarbeiter) können Sie auch verwenden. Er gibt direkt den Basisdatentyp aus.
#2.Ausgabe + Zuweisung
Anzahl_Mitarbeiter <- 17
```

`@sct`
```{r}
ex() %>% check_code(c("Anzahl_Mitarbeiter <- 17", "17->Anzahl_Mitarbeiter"), fixed=TRUE, missing_msg= "Nicht richtig. Schreiben Sie bitte den Code so, damit als Output 17 ausgeben wird!")
success_msg("Super, nun ist der richtige Wert zugewiesen worden!")
```

***

```yaml
type: NormalExercise
key: 845a69fe7e
xp: 30
```

`@instructions`
- 3. Ihr Chef Herr Müller hat für den Mitarbeiter Maximilian Flix ein neues Büro renovieren lassen. Nennen Sie das Büro **Office_33** bitte in **Nordwand** um.

`@hint`
Verweisen Sie auf die Variable Office_33 einfach den neuen Namen. Beachten Sie, dass Nordwand eine Zeichenkette (ein String) ist.

`@sample_code`
```{r}
#1.numerische Variable?
is.numeric(Anzahl_Mitarbeiter)
#2.Ausgabe + Zuweisung
print(Anzahl_Mitarbeiter)
Anzahl_Mitarbeiter <- 17
#3.Umbenennung Büro

```

`@solution`
```{r}

Office_33 <- "Nordwand"
```

`@sct`
```{r}
ex() %>% check_code(c(Office_33 <- "Nordwand", "Nordwand"-> Office_33), fixed=TRUE, missing_msg= "Da haben Sie etwas nicht richtig zugewisen. Verweisen Sie auf die Variable Office_33 den neuen Namen")
success_msg("Super - weiter geht´s, wir haben keine Zeit zu verlieren!")
```

---

## Vektoren

```yaml
type: TabExercise
key: 877cc6666f
xp: 100
```

Ein Vektor ist die einfachste Datenstruktur in R. Als "einzelnes Objekt, das aus einer Ansammlung von Daten besteht" wird ein Vektor im R-Handbuch definiert. Wir behandeln in dieser Einheit zum Einstieg nur numerische Vektoren, also Vektoren, die alle Arten von Zahlen enthalten können (de Vries/Meys 2018).

Um einen Vektor mit einer Folge von Zahlen von 1 bis 3 zu erzeugen:  
```
c(1,2,3) oder kürzer c(1:3)
```

Wichtige Befehle:

**str()**: Typ eines Vektors bestimmen und Überblick verschaffen.

**mean()**: Durchschnitt ausrechnen.

`@pre_exercise_code`
```{r}
sell.time <- c(8,8,8,8,9,6)
revenue.day <- c(2700, 3500, 4200, 4700, 5103, 3300)
```

***

```yaml
type: NormalExercise
key: 11c116d30a
xp: 25
```

`@instructions`
Sie sollen als Mitarbeiter der Business Intelligence & Data Analyticsabteilung erneut der kleinen Tochtergesellschaft zuarbeiten und analysieren dazu die Verkaufszeiten, den Umsatz pro Stunde und vergleichen diese auf Profitabilität.

- 1. Erstellen Sie einen Vektor, der die Zahlen von 1 bis 6 beinhaltet und weisen Sie ihm bitte den Variablennamen **open.vec** zu. Die Zahlen stehen jeweils für einen Verkaufstag (1 = "Montag")

`@hint`
Schauen Sie bitte in die Exercisebox dort sind Beispiele gegeben.

`@sample_code`
```{r}
# Verkaufstage

```

`@solution`
```{r}

open.vec <- c(1:6)
```

`@sct`
```{r}
ex() %>% check_object("open.vec") %>% check_equal("c(1,2,3,4,5,6)", "c(1:6)", fixed=TRUE, missing_msg="So ist das nicht ganz richtig!")
success_msg("Ja, genau!")
```

***

```yaml
type: NormalExercise
key: bcb2167aa1
xp: 25
```

`@instructions`
- 2. In dem Vektor **sell.time** ist die Verkaufszeit für jeden Verkaufstag hinterlegt. Lassen Sie sich bitte die Informationen über Typ und Struktur des Vektors **sell.time** ausgeben. Beurteilen Sie bitte, ob dieser nur numerische Zahlen enthält und welcher Tag der zeitlich längste ist.

`@hint`
Die Funktion **str()** haben Sie in der Kontextbeschreibung gegeben.

`@sample_code`
```{r}
#Verkaufszeit

```

`@solution`
```{r}

str(sell.time)
```

`@sct`
```{r}
ex() %>% check_code("str(sell.time)", fixed=TRUE, missing_msg="Verwenden Sie bitte die Funktionen aus der Kontextbeschreibung!") 
success_msg("Ja, genau. Die Funktion str() ist sehr hilfreich und verschafft Ihnen einen guten Überblick über den Vektor. Es ist nützlich, den Befehl immer im Hinterkopf zu behalten!")
```

***

```yaml
type: NormalExercise
key: 92d6aa8725
xp: 25
```

`@instructions`
- 3. Am Freitag wurden 5103 Euro Umsatz generiert. Wie viel wurde pro Stunde umgesetzt? Rechnen Sie es bitte aus.

`@hint`
Eine Divisionsaufgabe - denken Sie nicht kompliziert und tippen Sie es ein.

`@sample_code`
```{r}
# Umsatz pro Stunde am Freitag:

```

`@solution`
```{r}

5103/9
```

`@sct`
```{r}
ex() %>% check_output(567, fixed=TRUE, missing_msg="Nicht richtig, da haben Sie sich verrechnet!")
success_msg("Richtig. Am Freitag wurden 567€ Umsatz pro Stunde erwirtschaftet!")
```

***

```yaml
type: NormalExercise
key: c7fc94118a
xp: 25
```

`@instructions`
- 4. Berechnen Sie bitte die tägliche durchschnittliche Verkaufszeit pro Verkaufstag in der Woche.

`@hint`
Benutzen Sie die Funktion aus der Exercisebox und verwenden Sie die richtige Variable.

`@sample_code`
```{r}
# Durchschnittliche Verkaufszeit:

```

`@solution`
```{r}

mean(sell.time)
```

`@sct`
```{r}
ex() %>% check_output(7.833333, fixed=TRUE, missing_msg="Nicht ganz richtig!")
success_msg("Richtig - die durchnittliche tägliche Verkaufszeit beträgt 7,83 h!")
```

---

## Matrizen

```yaml
type: TabExercise
key: 2063bb6147
xp: 100
```

Vektoren in eine Matrix zusammenführen: 
- **rbind():** Funktion mit der Vektoren zu Zeilen ein und derselbe Matrix zusammengefügt werden können. *Matrix <- rbind(Vektor, Vektor)
- **cbind():** Funktion mit der Vektoren als Spalten einer Matrix zusammengefügt werden.

Werte einer Matrix ersetzen:
- Um den Wert in der dritten Zeile und zweiten Spalte der Matrix zu 5 zu ändern: my.matrix[3,2] <- 5

Zeilen- und Spaltennamen verändern: 
- Zeilennamen verändern: Bsp. **rownames(Matrix)** <- c("Region", "Umsätze")
- Spaltennamen verändern: Bsp. **colnames(Matrix)** <- c("Januar", "Februar")

`@pre_exercise_code`
```{r}
report.weeksales <- matrix(1:18, ncol=6)
report.final <- matrix(1:18, ncol=6)
sell.time <- c(8,88,8,8,9,6)
revenue.day <- c(2700, 3500, 4200, 4700, 5103, 3300)
average.byday <- c(2700/8, 3500/8, 4200/8, 4700/8, 5103/9, 3300/6)
```

***

```yaml
type: NormalExercise
key: ab3f22fb95
xp: 25
```

`@instructions`
Herr Müller bittet Sie einen Report mit dem Namen **report.weeksales** für die Tochterfirma zu erstellen.

- 1. Ihre Aufgabe ist es eine Matrix (Tabelle) aus den Vektoren **sell.time und revenue.day** zu erstellen und der Variable vom Typ Matrix **report.weeksales** zuzuordnen. Schauen Sie, ob Sie es richtig gemacht haben mit der Ausgabe in der Console.

`@hint`
Schauen Sie bitte in die Exercisebox und verwenden Sie bitte die Funktion um Zeilenvektoren zusammen zu führen und verweisen (<-) Sie diese auf report.weeksales.

`@sample_code`
```{r}
# report.weeksales

```

`@solution`
```{r}

report.weeksales <- rbind(sell.time, revenue.day)
```

`@sct`
```{r}
ex() %>% check_code(c("report.weeksales <- rbind(sell.time, revenue.day)", "rbind(sell.time, revenue.day) -> report.weeksales"), fixed=TRUE, missing_msg="Da stimmt etwas bei dem Erstellen der Matrix nicht. Verwenden Sie bitte die Funktionen aus der Kontextbeschreibung!") 
success_msg("Ja, genau - Schauen Sie sich gern Ihre selbst erstellte Tabelle an!")
```

***

```yaml
type: NormalExercise
key: 08550d114a
xp: 25
```

`@instructions`
- Sie haben den Report bei Herrn Müller abgegeben. Er kommt auf Sie zu und entgegnet Ihnen, ob Ihnen aufgefallen sei, dass sich noch ein Zahlenfehler eingeschlichen hat.

- 2. Lassen Sie sich die Matrix **report.weeksales** ausgeben und korrigieren Sie bitte den Report.

`@hint`
Haben Sie den falschen Wert entdeckt, ein Tag hat nur 24h! - Alles darüber ist falsch. report.weeksales[Zeile, Spalte] <- Wert

`@sample_code`
```{r}
# report.weeksales
report.weeksales <- rbind(sell.time, revenue.day)
#2.Ausgabe + Änderung vornehmen

```

`@solution`
```{r}
# Ausgabe
print(report.weeksales)
# Änderung vornehmen
report.weeksales[1,2] <- 8
```

`@sct`
```{r}
ex() %>% check_code(c("report.weeksales[1,2] <- 8","8 -> report.weeksales[1,2]"), fixed=TRUE, missing_msg="Der Code für die Änderung des Wertes ist nicht korrekt! Haben Sie die richtige Indizierung zur Korrektur des Wertes ausgewählt?") 
success_msg("Ja, genau - sonst wären falsche Umsatzzahlen an die Verkaufsniederlassung weitergegeben worden!")
```

***

```yaml
type: NormalExercise
key: cb0e656977
xp: 25
```

`@instructions`
- 3. Sie hatten für Freitag schon den durchschnittlichen Umsatz pro Stunde ausgerechnet. In dem Vektor **average.byday** wurde der Umsatz pro Stunde für alle sechs Verkaufstage errechnet. Fügen Sie dem Report bitte die Information des Vektors hinzu, damit der Wochenreport vollständig ist und weisen Sie den neuen Report bitte der Variablen **report.final** zu.

`@hint`
Bitte einen weiteren Vektor average.byday der Matrix hinzufügen. Die Funktion rbind() hatten Sie bereits in Teil 1 dieser Aufgabe verwendet.

`@sample_code`
```{r}
# report.weeksales
report.weeksales <- rbind(sell.time, revenue.day)
# Ausgabe + Änderung vornehmen
print(report.weeksales)
report.weeksales[1,2] <- 8
# Vektor hinzufügen

```

`@solution`
```{r}
report.final <- rbind(sell.time, revenue.day, average.byday) 
```

`@sct`
```{r}
ex() %>% check_code(c("report.final <- rbind(sell.time, revenue.day, average.byday)","report.final <- rbind(report.weeksales, average.byday)", "report.final <- rbind(average.byday, report.weeksales)"), fixed=TRUE, missing_msg= "Haben Sie den Vektor dem richtigen Teil der Tabelle zugewiesen? Verwenden Sie dazu bitte die Funktionen aus der Kontextbeschreibung!") 
success_msg("Ja, genau - der final Report ist fast fertig!")
```

***

```yaml
type: NormalExercise
key: 1a0c33c260
xp: 25
```

`@instructions`
Nun ist der Report für die Tochtergesellschaft schon fast fertig. Es fehlt noch eine eindeutige Benennung, damit dem Management der Tochtergesellschaft auf einen schnellen Blick ersichtlich ist, was dargestellt und analyisiert wurde. 

- 4. Bitte benennen Sie bei dem erstellten finalen Report die Zeilen- und Spaltennamen:
		
        - **Sales time in h, Revenue, Revenue per hour **
        - **Monday, Tuesday, Wednesday, Thursday, Friday, Saturday**

`@hint`
Schauen Sie dazu in die Exercisebox. Die Beispiele verdeutlichen die notwendige Programmierung sehr gut. Achten Sie darauf, dass die Bennenungen Zeichenketten sind.

`@sample_code`
```{r}
# report.weeksales
report.weeksales <- rbind(sell.time, revenue.day)
# Ausgabe + Änderung vornehmen
print(report.weeksales)
report.weeksales[1,2] <- 8
# Vektor hinzufügen
report.final <- rbind(sell.time, revenue.day, average.byday) 
# Tabelle benennen


```

`@solution`
```{r}
# Zeilennamen benennen
rownames(report.final) <- c("Sales time in h", "Revenue", "Revenue per hour")
## Spaltennamen bennen
#colnames(report.final) <- c("Monday","Tuesday", "Wednesday", "Thursday", "Friday", "Saturday")
```

`@sct`
```{r}
ex() %>% check_code(rownames(report.final) <- c("Sales time in h", "Revenue", "Revenue per hour"), fixed=TRUE, missing_msg="Haben Sie beachtet, dass die Benennungen Zeichenketten sind und dementsprechend gekennzeichnet werden müssen?") 
success_msg("Ja, genau! So behalten Sie die Übersicht und auch andere können Ihre Ergebnisse leichter nachvollziehen!")
ex() %>% check_code(colnames(report.final) <- c("Monday","Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"), fixed=TRUE, missing_msg=" Haben Sie alle Wochentage ohne Tippfehler und als Zeichenkette gekennzeichnet erstellt? Verwenden Sie bitte die Funktionen aus der Kontextbeschreibung") 
```

---

## Wrap-Up? Haben Sie es vertanden?

```yaml
type: PureMultipleChoiceExercise
key: 22c2d32180
xp: 50
```

14 %% 3

`@hint`
Überlegen Sie doch einmal. In Kaptitel 2 'Rechnen mit R' haben wir es besprochen.

`@possible_answers`
- 5
- 4
- 3
- [2]
- 1

`@feedback`
- "Nein, da haben Sie etwas falsch verstanden"
- "Nein, da liegen Sie nicht richtig"
- "Nein, da liegen Sie nicht richtig"
- "Super gemacht, 14 Modulo 3 ergibt 2" ![Glückwunsch](https://assets.datacamp.com/production/repositories/5050/datasets/9194e649dcb1fcbcdef15b71e344f1be3883fd18/Kurs%20Badge%202.jpg)
- "Nein, da liegen Sie nicht richtig"
