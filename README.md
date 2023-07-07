# GraphQl-Sample
- Base URI https://www.predic8.de/fruit-shop-graphql
- Request body_
query ($id: String!, $price: Float!) {
  products(id: $id, price: $price) {
    name
    price
    category {
      name
    }
    vendor {
      name
      id
    }
  }
}


-Response body_
{
  "data": {
    "products": [
      {
        "name": "Cherries",
        "price": 7.3,
        "category": {
          "name": "Fresh"
        },
        "vendor": {
          "name": "Home Fruits",
          "id": 501
        }
      }
    ]
  }
}

- Query variables_
{
  "id":"7",
  "price": 7.3
}
