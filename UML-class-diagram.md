classDiagram
    class Animal {
        - name: String
        + Animal(name: String)
        + getName(): String
        + makeSound(): String
    }
    class Dog {
        - breed: String
        + Dog(name: String, breed: String)
        + getBreed(): String
        + makeSound(): String
        + fetch(): void
    }
    class Cat {
        - lives: int
        + Cat(name: String)
        + getLives(): int
        + makeSound(): String
        + loseLive(): void
    }
    class Bird {
        - canFly: boolean
        + Bird(name: String, canFly: boolean)
        + getCanFly(): boolean
        + makeSound(): String
        + fly(): void
    }

    Animal <|-- Dog
    Animal <|-- Cat
    Animal <|-- Bird

    class Animal abstract
