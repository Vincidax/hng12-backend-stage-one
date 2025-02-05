# Number Classification API

This API classifies numbers by determining various mathematical properties such as whether they are prime, perfect, Armstrong, or even/odd. Additionally, it provides a fun fact about the number fetched from the Numbers API.

## API Overview

### Endpoint:

- **GET** `/api/classify-number?number={number}`

### Parameters:

- `number`: The number to be classified (required, must be a valid integer).

### Response:

- The API will return a JSON response containing the following information:
  - `number`: The number provided in the request.
  - `is_prime`: Boolean indicating whether the number is prime.
  - `is_perfect`: Boolean indicating whether the number is a perfect number.
  - `properties`: An array containing properties of the number (e.g., "armstrong", "odd", "even"). Possible values include "prime", "perfect", "armstrong", "even", "odd".
  - `digit_sum`: The sum of the digits of the number.
  - `fun_fact`: A fun fact about the number (from the Numbers API).

### Example Requests and Responses:

```http
GET [https://hng12-backend-stage-one.vercel.app/api/classify-number?number=371](https://hng12-backend-stage-one.vercel.app/api/classify-number?number=371)
```
