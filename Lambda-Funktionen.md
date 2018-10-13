# Was ist eine Lambda-Funktion?

## Definition
Lambda-Funktionen sind kleine, anonyme Funktionen, d.h. ihnen wird kein Name zugewiesen. Diese Funktionen können zum Beispiel für einfache Rechenoperationen herangezogen werden.

Lambda-Funktionen werden verwendet, wenn Funktionen nur einmal verwendet werden.

Lambda-Funktionen können auch innerhalb von anderen Funktionen aufrufen werden.

## Syntax
**lambda** *Parameterliste* : *arithmetischer Ausdruck*

Hinweis: Die Parameterliste kann mehrere Werte umfassen.

Zum Beispiel:
s = lambda a : a + 10 - Diese Funktion erhöht den Wert von a um 10.

Aufgerufen wird die Funktion mit s(5). Zurückgeliefert wird das Ergebnis 15.


## Anwendungsbeispiele

    s = lambda a : a + 10 │ s(a) liefert einen Wert von a + 10 zurück.
    print(s(5))
    
    ► Ergebnis: 15


    x = lambda a, b : a * b │ x(a,b) liefert das Produkt der Multiplikation von a und b zurück.
    print(x(5, 6))
    
    ► Ergbnis: 30


    x = lambda a, b, c : a + b + c │ x(a,b,c) liefert die Summe der drei Argumente zurück.
    print(x(5, 6, 2))
    
    ► Ergebnis: 13


    def myfunc(n):
      return lambda a : a * n

    mydoubler = myfunc(2)

    print(mydoubler(11))
    
    ► Ergebnis: 22
    
    
    def myfunc(n):
        return lambda a : a * n

        mydoubler = myfunc(2)
        mytripler = myfunc(3)

        print(mydoubler(11)) 
        print(mytripler(11))
        
     ► Ergebnis: 22 und 33
        
      
     sorted([1,4,7,3,5], key = lambda x : -x
     
     ► Ergebnis: [7, 5, 4, 3, 1]
     
     
     s = lambda x: True if x % 2 == 0 else False
     
     print (s(10))
     print (s(11))
     
     ► Ergebnis: True und False
     
     
     s = lambda x: ‘big’ if x > 100 else ‘small’
     
     print (s(200))
     
      ► Ergebnis: 'big'
     
     
     
     
