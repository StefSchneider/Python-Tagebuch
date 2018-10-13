# Was ist eine Lambda-Funktion?

## Definition
Lambda-Funktionen sind kleine, anonyme Funktionen, d.h. ihnen wird kein Name zugewiesen. Diese Funktionen können zum Beispiel für einfache Rechenoperationen herangezogen werden.

Lambda-Funktionen können auch innerhalb von anderen Funktionen aufrufen werden.

## Syntax
**lambda** *Parameterliste* : *arithmetischer Ausdruck*

Hinweis: Die Parameterliste kann mehrere Werte umfassen.

Zum Beispiel:
s = lambda a : a + 10 - Diese Funktion erhöht den Wert von a um 10.

Aufgerufen wird die Funktion mit s(5). Zurückgeliefert wird das Ergebnis 15.


## Anwendungsbeispiele

    s = lambda a : a + 10    s(a) liefert einen Wert von a + 10 zurück.
    print(s(5))

    x = lambda a, b : a * b     x(a,b) liefert das Produkt der Multiplikation von a und b zurück.
    print(x(5, 6))

    x = lambda a, b, c : a + b + c      x(a,b,c) liefert die Summe der drei Argumente zurück.
    print(x(5, 6, 2))


    def myfunc(n):
      return lambda a : a * n

    mydoubler = myfunc(2)

    print(mydoubler(11))
