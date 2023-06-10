@startuml
scale 3
class Animal{
    -nombre: string
    -lugarOrigen: string
    -color: string
    +sonido(String): void
    +comer(): void
    
}

class AnimalAcuatico{
    -numeroAletas: int
    +nadar(): void
    +comer(): void
}

Animal <|-- AnimalAcuatico

class Ballena{
    -largo:int
    +peleaConPinocho(): void
}

AnimalAcuatico <|--- Ballena

class AnimalTerrestre{
    -numeroPatas: int
    +correr(): void
    +comer(): void
}

Animal <|-- AnimalTerrestre

class Perro{
    -colorCollar: string
    +hacerTrucos(): void
}

AnimalTerrestre <|--- Perro

class AnimalAereo{
    -numeroAlas: int
    +volar(): void
    +comer(): void
}

Animal <|-- AnimalAereo

class Pajaro{
    -tipoPico: string
    +recolectarRamas(): void
}

AnimalAereo <|--- Pajaro



