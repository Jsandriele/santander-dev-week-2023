#Santander Dev Week 2025
Java Restful API criada para a Santander Dev week


##Diagrama de Classes



```mermaid
classDiagram
    class User {
        +String name
        +Account account
        +List~Feature~ features
        +Card card
        +List~News~ news
    }
    
    class Account {
        +String number
        +String agency
        +String balance
        +String limit
    }
    
    class Feature {
        +String icon
        +String description
    }
    
    class Card {
        +String number
        +String limit
    }
    
    class News {
        +String icon
        +String description
    }
    
    User "1" --> "1" Account
    User "1" --> "n" Feature
    User "1" --> "1" Card
    User "1" --> "n" News
```
