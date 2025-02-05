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

**GET** [https://hng12-backend-stage-one.vercel.app/api/classify-number?number=371](https://hng12-backend-stage-one.vercel.app/api/classify-number?number=371)
### Number 371
- **Is Prime**: No
- **Is Perfect**: No
- **Properties**: Armstrong, Odd
- **Digit Sum**: 11
- **Fun Fact**: 371 is an Armstrong number because \(3^3 + 7^3 + 1^3 = 371\).

### Error Handling
The API returns standard HTTP status codes to indicate the success or failure of a request. Here's a breakdown of potential error responses:

| Status Code | Description                               | Example Response                                                      |
|-------------|-------------------------------------------|----------------------------------------------------------------------|
| 400         | Bad Request - Invalid input (e.g., non-integer number) | `{"number": "abc", "error": true}` |

### Features:
- **Prime Check**: Determines if a number is prime.
- **Perfect Number Check**: Determines if the number is a perfect number.
- **Armstrong Number Check**: Verifies if a number is an Armstrong number.
- **Digit Sum**: Computes the sum of the digits of the number.
- **Properties**: Returns the properties of the number such as Armstrong, Odd, or Even.
- **Fun Fact**: Fetches a fun fact from the Numbers API (with attribution to the Numbers API).

### Installation
To set up this API locally, follow these steps:

#### Prerequisites:
- **Node.js**: Ensure Node.js is installed on your machine.

#### Clone the repository:
```bash
git clone [https://github.com/Vincidax/hng12-backend-stage-one.git](https://github.com/Vincidax/hng12-backend-stage-one.git)
cd hng12-backend-stage-one

#### Install dependencies:
To install the necessary dependencies, run the following command:

```bash
npm install

#### Start the server:
To start the server, run the following command:

```bash
node index.js

### Deployment
This project is deployed on Vercel. You can access the API at the following URL:

[https://hng12-backend-stage-one.vercel.app/api/classify-number](https://hng12-backend-stage-one.vercel.app/api/classify-number)

### License
This project is open-source and available under the MIT License.

### Contribution
Author: Vincent DUSHIME
