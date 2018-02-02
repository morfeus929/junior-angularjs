## Required Technologies
 - AngularJS
 - Bootstrap/Material
 - Gulp/Grunt/Webpack

## Getting Started

###### Install npm dependencies
`npm install`

###### Run the node server
`node app.js`

###### Viewing the application in your browser
`http://localhost:8000`


## Resources

#### Customers
```
GET|POST          /api/customers
GET|PUT|DELETE    /api/customers/{id}

{
  'id': integer
  'name': string
  'address': string
  'phone': string
}
```

#### Products
```
GET|POST          /api/products
GET|PUT|DELETE    /api/products/{id}

{
 'id': integer
 'name': string
 'price': decimal
}
```
#### Invoices
```
GET|POST          /api/invoices
GET|PUT|DELETE    /api/invoices/{id}

{
 'id': integer
 'customer_id': integer
 'discount': decimal
 'total': decimal
}
```

#### InvoiceItems
```
GET|POST          /api/invoices/{id}/items
GET|PUT|DELETE    /api/invoices/{invoice_id}/items/{id}

{
 'id': integer
 'invoice_id': integer
 'product_id': integer
 'quantity': decimal
}
```
