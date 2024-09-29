# Mermaid Diagram
## Entity Relationship Diagram

```mermaid
erDiagram

  CUSTOMER ||--o{ SALE: places
  CUSTOMER ||--|{ PERSON: Info
  CUSTOMER {
  string name
  string custNumber PK
  string sector
  }

  PERSON {
  String(99) firstName "Up to 99 characters"
  String(99) lastName "Up to 99 characters"
  String phone UK
  String email
  String address
}
  
  SALE ||--o{ INVENTORY: Product
  SALE {
  String prodNumber
  Int orderNumber
  String deliveryAddress
  }
  
  INVENTORY ||--o{ PRODUCT: Type
  INVENTORY {
  String prodNumber
  int quantity
  float PricePerUnit
  }

  PRODUCT {
  String name
  String prodNumber
  String Cost
  }
  
 
 ```

