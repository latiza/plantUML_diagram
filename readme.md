https://plantuml.com/

A PlantUML egy szöveg-alapú eszköz UML diagramok készítésére, amely lehetővé teszi, hogy a diagramokat kód segítségével definiáld. Ahelyett, hogy a diagramot vizuálisan húznád össze, egyszerű szintaxissal írhatod le, hogyan nézzen ki, és a PlantUML automatikusan megrajzolja neked. A kódja egyszerű és gyorsan tanulható, így ideális UML diagramok gyors készítéséhez és verziókezeléséhez.

Alapvető Nyelvi Szintaxis a PlantUML-ban
A PlantUML szintaxis egyszerű, és hasonlít a természetes nyelvre:

Minden diagramot az @startuml és az @enduml kulcsszavak közé kell írni.
Használhatsz kulcsszavakat, mint például actor, class, interface, start, stop, és ezekkel megadhatod a diagram elemeit és azok kapcsolatait.

Példák:
Osztálydiagram:

@startuml
class Auto {
    - motor: String
    + elindit()
    + megall()
}
class Motor
Auto -- Motor : tartalmaz
@enduml

Aktivitásdiagram:

@startuml
start
:Felhasználó bejelentkezik;
:Termék kiválasztása;
if (Kosár üres?) then (igen)
    :Kosár frissítése;
else (nem)
    :Tovább a fizetéshez;
endif
stop
@enduml