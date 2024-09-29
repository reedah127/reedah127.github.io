# Mermaid Diagram
## Entity Relationship Diagram
For the relationship I put customer first, here we can see I put the customer number as well as the location and name. From there you can go two ways, to person and sale. For person this is more info for the customer, incuding name, age, address, and email. The sale is then what is needed to help the store which is the product number, order number and the delivery address. Connected to that we have inventory of the store which is connected to product. The inventory is needed for quantity and to see what products they actually have in the store as well as item number. Last is product which is price of the item and more details of the product itself. 

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
  String prodDescription
  }
  
 
 ```

