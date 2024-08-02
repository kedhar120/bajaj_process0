# Bajaj Finserv Health Dev Challenge

## Overview

This repository contains the solution for the Bajaj Finserv Health Dev Challenge. The challenge involves building and deploying a full-stack application with both backend and frontend components.

## Backend

The backend is a REST API with a single endpoint /bfhl that supports both GET and POST methods.

### Endpoints

- *POST /bfhl*
  - Accepts a JSON payload and returns a response with status, user ID, email, roll number, arrays of numbers and alphabets, and the highest alphabet.
  - Example Request:
    json
    {
      "data": ["M", "1", "334", "4", "B"]
    }
    
  - Example Response:
    json
    {
      "is_success": true,
      "user_id": "john_doe_17091999",
      "email": "john@xyz.com",
      "roll_number": "ABCD123",
      "numbers": ["1", "334", "4"],
      "alphabets": ["M", "B"],
      "highest_alphabet": ["M"]
    }
    

- *GET /bfhl*
  - Returns a hardcoded operation code.
  - Example Response:
    json
    {
      "operation_code": 1
    }
    

### Hosting

The backend can be hosted on any provider such as Heroku, Netlify, Vercel, or Firebase. For this example, Heroku is used.

## Frontend

The frontend is a web application that interacts with the backend API to process input and render the response. It is built using React.

### Features

1. *Text Input Field and Submit Button*
   - Accepts valid JSON input.
   - Validates JSON format on submission.
   - Calls the backend API with the input data.
   - Renders the response.

2. *Multi-Select Dropdown*
   - Appears after valid JSON submission.
   - Options: Alphabets, Numbers, Highest Alphabet.
   - Filters and displays the response based on selected options.

3. *Website Title*
   - The title of the website is set to your roll number.

### Example Usage

- After submitting the JSON { "data": ["A", "C", "z"] }, the user can select options from the dropdown to filter the response.
- If "Numbers" and "Highest Alphabet" are selected, the response will display numbers and the highest alphabet from the input data.

## Submission

1. Host the backend and frontend applications.
2. Share the backend API endpoint (ending in /bfhl) and the frontend application URL in the provided form.
3. The fastest valid submissions will be considered.

## Links

- [Backend API Endpoint](#) (replace with actual URL)
- [Frontend Application URL](#) (replace with actual URL)
- [Submission Form](https://forms.office.com/r/kgwxTBPnCw)

## Notes

- Ensure best practices including exception handling and input validation are followed.
- Do not forward the challenge document.

---

This solution is developed as part of the Bajaj Finserv Health Dev Challenge (Qualifier 1) organized by SRM University on 2nd August 2024.
