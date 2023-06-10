@startuml
scale 3
class AplicationUser{
    -userName: string
    -password: string
    +islocked: boolean
    -suggestRandomPassword()
    +changeProfilePic()
}

abstract class Event{
    +startTime: DateTime
    +venue: string
    registrationClosed: bolean
    -notifyAttendes()
}

interface Hola{
    +perro: int
    -gato: float
    +pericoMuerde()

}

class Saludar{
    +buenDia: String
}
Hola <|-- Saludar: implements
@enduml