## Simple Animal Object-Oriented Program (OOP)

### Animal Class
The `Animal` class serves as the base class for various animals. It has the following properties and methods:

- **Properties:**
  - `color`: Represents the color of the animal (default is "yellow").
  - `energy`: Represents the energy level of the animal (default is 100).

- **Methods:**
  - `isActive()`: Checks if the animal is active based on its energy level. If energy is greater than 0, it decreases energy by 20. If energy is 0, it calls the `sleep` method.
  - `sleep()`: Increases the energy level of the animal by 20.
  - `getColor()`: Logs the color of the animal.

### Cat Class (extends Animal)
The `Cat` class extends the `Animal` class, inheriting its properties and methods. It introduces additional properties specific to cats:

- **Additional Properties:**
  - `sound`: Represents the sound the cat makes (default is "purr").
  - `canJumpHigh`: Indicates if the cat can jump high (default is `true`).
  - `canClimbTrees`: Indicates if the cat can climb trees (default is `true`).

- **Additional Method:**
  - `makeSound()`: Logs the sound the cat makes.

### Bird Class (extends Animal)
The `Bird` class extends the `Animal` class, inheriting its properties and methods. It introduces additional properties specific to birds:

- **Additional Properties:**
  - `sound`: Represents the sound the bird makes (default is "chirp").
  - `canFly`: Indicates if the bird can fly (default is `true`).

- **Additional Method:**
  - `makeSound()`: Logs the sound the bird makes.

### HouseCat Class (extends Cat)
The `HouseCat` class extends the `Cat` class, inheriting properties and methods from both `Cat` and `Animal`. It introduces an additional property specific to house cats:

- **Additional Property:**
  - `houseCatSound`: Represents the sound the house cat makes (default is "meow").

- **Override Method:**
  - `makeSound(option)`: Overrides the `makeSound` method from the `Cat` class. If `option` is `true`, it calls the `makeSound` method from the `Cat` class. Then, it logs the house cat sound.

### Tiger Class (extends Cat)
The `Tiger` class extends the `Cat` class, inheriting properties and methods from both `Cat` and `Animal`. It introduces an additional property specific to tigers:

- **Additional Property:**
  - `tigerSound`: Represents the sound the tiger makes (default is "Roar!").

- **Override Method:**
  - `makeSound(option)`: Overrides the `makeSound` method from the `Cat` class. If `option` is `true`, it calls the `makeSound` method from the `Cat` class. Then, it logs the tiger sound.

### Parrot Class (extends Bird)
The `Parrot` class extends the `Bird` class, inheriting properties and methods from both `Bird` and `Animal`. It introduces an additional property specific to parrots:

- **Additional Property:**
  - `canTalk`: Indicates if the parrot can talk (default is `false`).

- **Override Method:**
  - `makeSound(option)`: Overrides the `makeSound` method from the `Bird` class. If `option` is `true`, it calls the `makeSound` method from the `Bird` class. If the parrot can talk, it logs a message indicating that it's a talking parrot.

### Object Instantiations and Method Calls
- Objects of various classes (e.g., `Parrot`, `Bird`, `HouseCat`) are instantiated with specific configurations.
- Methods such as `makeSound` and `isActive` are called on these objects to demonstrate their behavior.

This code demonstrates the use of inheritance, polymorphism, and encapsulation, fundamental concepts in object-oriented programming, to model different types of animals with shared and unique characteristics.
