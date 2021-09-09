# Drawbot Cheatsheet

## Kurzbefehle

`cmd r` Programm ausführen

`cmd alt 5` Zeile ausrücken

`cmd alt 6` Zeile einrücken

`cmd alt 8` Zeile deaktivieren

`cmd alt 9` Zeile aktivieren

`cmd Pfeiltaste` Wert ausgewählter Zahl ändern

## Variablen

`foo = 12` Wertzuweisung

`foo = foo + 1` Wert in Variable um 1 erhöhen

`foo += 1` Wert in Variable um 1 erhöhen (Kurzschreibweise)

`foo = foo - 1` Wert in Variable um 1 reduzieren

`foo -= 1` Wert in Variable um 1 reduzieren (Kurzschreibweise)

## Rechnen

`+` Addition

`-` Subtraktion

`*` Multiplikation

`/` Division, mit Resultat mit Kommastellen

`//` Division, mit ganzer Zahl als Resultat (gerundet)

`%` Modulo (Rest der Division)

## Nützliche Python-Funktionen

`print()` Output in Konsolen-Fenster schreiben

`randint(A, B)` zufällige ganze Zahl zwischen A und B

`random()` zufällige Zahl zwischen 0 und 1

`range(7)` generiert die Liste `[0, 1, 2, 3, 4, 5, 6]`

`range(4, 7)` generiert die Liste `[4, 5, 6]`

`range(2, 7, 2)` generiert die Liste `[2, 4, 6]`

## Die wichtigsten Drawbot-Funktionen

`newPage(w, h)` generiert eine neue Seite in Print-Dokumenten, bzw. ein neues Frame in Animationen. Angaben in Zahlen ergeben Punkte für PDF, bzw. Pixel für GIF, PNG etc. Möglich sind auch Angaben wie `"A4"` oder `"A0Landscape"`, siehe [Drawbot-Doku](https://www.drawbot.com/content/canvas/pages.html?highlight=newpage).

`width()` liefert die Breite der Hintergrundfläche

`height()` liefert die Höhe der Hintergrundfläche

`oval(x, y, w, h)` zeichnet ein Oval, bzw. einen Kreis, wenn w = h

`rect(x, y, w, h)` zeichnet ein Rechteck

`line((x1, y1), (x2, y2))` zeichnet eine Linie. Die Funktion `line()` braucht als Argumente **zwei Klammern** mit den Positionen zweier Punkte.

`font("Times-Italic", 200)` stellt Font und Schriftgrösse ein. Als Name muss der sog. «Postscript-Name» des Fonts angegeben werden. Das ist meist der Dateiname ohne Endung, kann aber auch in der Schriftsammlung unter den Infos zum Font nachgeschaut werden.

`fill(0)` stellt die Füllfarbe ein. Werte von 0–1.

- Ein einziger Wert bezieht sich auf **Graustufen**
- zwei Werte auf **Graustufen und Transparenz**
- drei Werte auf **RGB**
- vier Werte auf **RGB und Transparenz**.
- zum Umrechnen 255-Stufige RGB-Werte **durch 255 teilen**
- `None` ist auch ein gültiger Wert.

`stroke()` stellt Linienfarbe ein. Wenn nicht angegeben, auf `stroke(None)` eingestellt.

`strokeWidth()` Die Strichstärke in Punkt.

## Schleifen

    for text in ["lorem", "ipsum"]:
        print(text)

    for var in range(10):
        print(var)


## Bedingungen

    if random() > 0.66:
        print("Schere")
    elif random() > 0.33:
        print("Stein")
    else:
        print("Papier")

## Reservierte Wörter

… die nicht als Variablen verwendet werden dürfen:

- and
- del
- from
- not
- while
- as
- elif
- global
- or
- with
- assert
- else
- if
- pass
- yield
- break
- except
- import
- print
- class
- exec
- in
- raise
- continue
- finally
- is
- return
- def
- for
- lambda
- try