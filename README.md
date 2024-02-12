# Santander Dev Week

## Diagrama de classes
```mermaid
classDiagram
class User {
  name: String
  account: Account
  features: Feature[]
  card: Card
  news: News[]
}

class Account {
  number: String
  agency: String
  balance: number
  limit: number
}

class Feature {
  name: String
  description: String
  icon: URL
}

class Card {
  number: String
  type: String
  limit: Number
  expirationDate: Date
}

class News {
  title: String
  description: String
  icon: URL
}


User "1" *-- "1" Account
User "1" *-- "N" Feature
User "1" *-- "1" Card
User "1" *-- "N" News
```
