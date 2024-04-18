    classDiagram
```mermaid
    Weapon <|-- Sword
    Weapon <|-- Gun
    Player <|-- Gun
    Enemy <|-- Gun

    Gun <-- Player 
    Sword <-- Player
    Weapon <-- Player
    Player <-- Program
    Enemy <-- Program
    Program <-- Character

    Weapon o-- Character

    class Player{
        Name: str
    }

    class Gun{
        Ammo: int
    }

    class Sword{
        BladeLenght: float
        Power: float
    }

    class Program{
    }

    class Character{
        Weapon: str
        Name: str
    }

    class Weapon{
        Power: float
    }

    class Enemy{
        Name: str
    }