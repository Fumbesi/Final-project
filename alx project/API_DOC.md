Ndlovu Calculator API Documentation
Introduction
The Ndlovu Calculator API allows users to perform various mathematical calculations such as addition, subtraction, multiplication, division, trigonometric functions, and more.

Base URL
arduino
Copy code
https://example.com/calculator

Endpoints
Perform Calculation
URL: /calculate
Method: POST
Description: Performs a mathematical calculation based on the provided expression.

Request Body:
expression (string, required): The mathematical expression to be evaluated.

Response:
result (number): The result of the calculation.
error (string, optional): If an error occurs during the calculation, an error message will be provided.

Request Example
json
Copy code
POST /calculate
Content-Type: application/json

{
    "expression": "2 + 2 * (3 - 1)"
}

Response Example
json
Copy code
HTTP/1.1 200 OK
Content-Type: application/json

{
    "result": 6
}
