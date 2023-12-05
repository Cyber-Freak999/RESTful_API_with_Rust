# Rust Warp Grocery List API
This is a simple Rust application built using the Warp framework to manage a grocery list through HTTP endpoints.

# Features
- Add items to the grocery list
- Get the entire grocery list
- Update item quantity on the grocery list
- Delete items from the grocery list

# Installation and Usage
## Prerequisites
[Rust](https://www.rust-lang.org/) installed on your system
## Setup
1. Clone the repository:

```bash
git clone https://github.com/your-username/rust-warp-grocery-list.git
cd rust-warp-grocery-list
```

2. Run the application:

```bash
cargo run
```
3. The application will start at http://localhost:3030.

# Endpoints
## Add Items to Grocery List
### POST /v1/groceries
Add items to the grocery list:
- Request body should contain JSON with name and quantity fields.
	
## Get Grocery List
### GET /v1/groceries
Retrieve the entire grocery list.

## Update Item Quantity
### PUT /v1/groceries
Update item quantity on the grocery list:
- Request body should contain JSON with name and quantity fields.
	
## Delete Item from Grocery List
### DELETE /v1/groceries
Remove item from the grocery list:
- Request body should contain JSON with name field.

# API Payloads
## Add/Update Item Payload
```json
{
  "name": "ItemName",
  "quantity": 5
}
```
## Delete Item Payload
```json
{
  "name": "ItemName"
}
```