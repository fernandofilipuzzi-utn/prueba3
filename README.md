# Diagrama de clases - UML

```plantuml
@startuml

class Persona {
    -nombre: String
    -edad: int
    +hablar(): void
}

class Estudiante extends Persona {
    -legajo: String
    +estudiar(): void
}

@enduml
