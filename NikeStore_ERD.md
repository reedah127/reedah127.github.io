erDiagram
  PRODUCT ||--o{ CUSTOMER
  PRODUCT {
  String name
  String prodNumber
  String Cost
  }
  
  CUSTOMER ||--o{ SALE: places
  CUSTOMER {
  string name
  string custNumber
  string sector
  }
  
  SALE ||--|{ INVENTORY
  SALE {
  String prodNumber
  Int orderNumber
  String deliveryAddress
  }
  
  INVENTORY {
  String prodNumber
  }
