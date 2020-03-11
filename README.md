# plantUMLstyle
A style for plantUML

## Usage

### Dark theme
Code example for dark theme
```
@startuml
!define DARK
!includeurl https://raw.githubusercontent.com/XaBerr/plantUMLstyle/master/style.plantuml
' your code here
@enduml
```

```plantuml
@startuml
!define DARK
!includeurl https://raw.githubusercontent.com/XaBerr/plantUMLstyle/master/style.plantuml
abstract class Animal {
  - name: String
  - age: int
  - family: String
  - gender: bool
  --
  + setName()
  + setAge()
  + setFamily()
  + setGender()

  + getName(): String
  + getAge(): int
  + getFamily(): String
  + getGender(): bool

  + eat( food )
}

class Penguin {
  - type: String
  
  + setType()

  + getType(): String
}
note left of Penguin: type can be\n(skipper, soldato, kowasky, riko)

class Cage {
  - size: vector<int, int>
  - maxNumAnimals: int
  
  + setType()
  + setMaxNumAnimals(): vector<int, int>
  
  + getType()
  + getMaxNumAnimals(): int
}

Animal <|-- Penguin
Animal <|-- Cat
Animal <|-- Otter

Animal "a 2..*" o-left-- "c 1..*" Cage
@enduml
```
![zooDark](https://user-images.githubusercontent.com/16030020/76464158-16d5ea80-63e5-11ea-9d14-1e413b408d42.png)

### Light theme
Code example for light theme.
```
@startuml
!define LIGHT
!includeurl https://raw.githubusercontent.com/XaBerr/plantUMLstyle/master/style.plantuml
' your code here
@enduml
```

```plantuml
@startuml
!define LIGHT
!includeurl https://raw.githubusercontent.com/XaBerr/plantUMLstyle/master/style.plantuml
abstract class Animal {
  - name: String
  - age: int
  - family: String
  - gender: bool
  --
  + setName()
  + setAge()
  + setFamily()
  + setGender()

  + getName(): String
  + getAge(): int
  + getFamily(): String
  + getGender(): bool

  + eat( food )
}

class Penguin {
  - type: String
  
  + setType()

  + getType(): String
}
note left of Penguin: type can be\n(skipper, soldato, kowasky, riko)

class Cage {
  - size: vector<int, int>
  - maxNumAnimals: int
  
  + setType()
  + setMaxNumAnimals(): vector<int, int>
  
  + getType()
  + getMaxNumAnimals(): int
}

Animal <|-- Penguin
Animal <|-- Cat
Animal <|-- Otter

Animal "a 2..*" o-left-- "c 1..*" Cage
@enduml
```

![zooLight](https://user-images.githubusercontent.com/16030020/76464098-fc9c0c80-63e4-11ea-80a4-b75e789820ef.png)