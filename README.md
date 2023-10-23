# API Java RESTful API

## Diagrama de Classes 

```mermaid
classDiagram
    class User {
        - String name
        - Account account
        - List<Feature> features
        - Card card
        - List<News> news
        - String newsIcon
        - String newsDescription
    }

    class Account {
        - String accountNumber
        - String accountAgency
        - Number accountBalance
        - Number accountLimit
    }

    class Feature {
        - String icon
        - String description
    }

    class Card {
        - String cardNumber
        - Number cardLimit
    }

    class News {
        - String icon
        - String description
    }

    User "1" *-- "1" Account : has
    User "1" *-- "N" Feature : has many
    User "1" *-- "1" Card : has
    User "1" *-- "N" News : has many
```

