# Was sind Annotationen?

Annotationen sind Ergänzungen zu Parametern einer Funktion oder zu Variablen. Sie legen fest, um welchen Datentyp es sich dabei handelt. Annatation können deshalb auch gut zu Kontrollzwecken eingesetzt werden: Werden Parameter eines nicht gültigen Datentyps übergeben oder entspriccht der Rückgabewert einer Funktion nicht dem Datantyp, wird eine Fehlermeldung erzeugt. 

Annatitionen können damit den Code lesbarer für andere Entwickler machen, da sie direkt den Datentyp der einzelnen Parameter und Variablen verdeutlichen.

# Syntax

Annotation werden direkt hinter den einzelnen Parameter gesetzt. Dazwischen steht ein Doppelpunkt:

parameter: Annotation

Auch hinter den Funktionskopf kann eine Annotation gesetzt werden, um den Rückgabewert zu überprüfen. Dann wird die Annotation mit '->' eingeleitet_

**def** funktion -> Annotation:

Wichttig: Der Doppelpunkt zum Ende eines Funktionskopfes kommt erst nach der Annotation.

Eine Funktion wird also wie folgt mit Annotationen versehen:

**def** funktion(*parameter1*: Annotation1, *parameter2*: Annotation2) -> Annotation3:  

    *Funktionskörper*
    
Auch für Variablen können Annotationen verwendet werden. Sie werden ebenso wié bei den Funktionsparametern direk hinter den Variablennamen geschrieben.

variable: Annotation

Zusätzlich können die Variablen mit einem direkten Wert versehen werden:

variable: Annotation = 10

In diesem Fall erhält 'variable' den Wert 10.

# Annotationsabkürzungen

- int: Integer
- set: Set
- str: String
- list: Liste
- dict: Dictionary
- frozentset: Frozenset
  
