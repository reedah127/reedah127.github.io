erDiagram
  PRODUCT ||--o{ 
  PRODUCT {
  String name
  String prodNumber
  String Cost
  CUSTOMER ||--o{ ORDER: places
  CUSTOMER {
  string name
  string custNumber
  string sector
  }
  SALE ||--o{ 
  SALE {
  String prodNumber
  Int orderNumber
  }
  INVENTORY {
  String prodNumber
  }
