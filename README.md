# Inheritance-and-Composition
Session 8

### Assignment

#### Idea

Implement a **Zoo Management System** where all the animals will be allocated to zones based on their characteristics. 

Note that the focus of this problem is on design of related classes. It involves identifying classes, their attributes and methods, taking decision about where to implement/override methods, how to organise related objects into a structure etc. There may be multiple alternatives for design, each having its own advantages and disadvantages. 

#### Details

Create a hierarchy of animal where Animal is the base class and its subclasses could be various categories of animals like Mammal, Reptile, Bird, etc. Each of these classes can have further subclasses representing the specific types of animal like  Lion, Crocodile, Peacock, etc. 

The Zoo Management System will have multiple zones and each zone would support animals from a single category like mammal, reptile or bird. There could be multiple zones for the same category. Each zone will have cages for animals. Each zone has a limit on the number of cages that can be added to the zone. A zone could have additional attributes like hasPark, hasCanteen etc.

Each cage will specify the type of animals that can be added to the cage, and will have a limit on the number of animals that can be added to the cage.

When a new animal is added to the zoo, it will be allocated to an existing cage if there is available capacity. Otherwise a new cage will need to be added. 

Each animal will have a unique name, and will have attributes like age, weight etc. It will support methods like getSound() which returns a string representing the sound corresponding to that animal type, like for a lion it should return “roars”. 

#### Operations

a) A cage should specify a) the type of animals that can be added to it like tiger, and b) its capacity.

b) An animal can only be allocated to an existing cage based on available capacity. The system can allocate cage automatically.

c) Allow addition of one animal at a time, and if there is no capacity available then the operation should fail.

d) Each animal should be assigned a unique name, which is a string. Internal id can be assigned automatically.

e) Allow for death of an animal, where the animal will get removed from the zoo.

f) Provide the operation to add a cage to a zone.

g) Instead of asking methods to print/display, return values. UI is not part of this class

