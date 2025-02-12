# Overview

PyMonday is a monday.com API Python Client Library, compatible with API version 2025-01 and later.

---

## Official API Documentation

<a href='https://developer.monday.com/api-reference/docs/basics'>Monday API Documentation</a>

---

## Installation

To install pymonday, use the following pip command in your project virtual environment.

```bash
pip install pymonday
```

---

## API Authentication

You must pass your monday.com API key to the MondayAPIClient object to authenticate API calls.

Review the Official API Documentation for instructions on obtaining an API Key. 

---

## Instantiate Client Object

To import the monday.com API client into your project, use the following import statement:
```python
from pymonday import MondayAPIClient
```

An instance of the API Client Object can then be created:
```python
monday = MondayAPIClient(api_key="API_KEY")
```

---

## Using MondayAPIClient

The **`MondayAPIClient`** provides a streamlined interface for interacting with the **Monday.com API**, organizing 
functionality into intuitive method groups. Users can access different features, such as managing boards, items, users, 
and updates, through dedicated attributes on the client instance. For example, you can retrieve account details using 
`monday.account.get_account_details()` or fetch items from a board using `monday.items.get_items_from_column()`.

Each method group handles specific API operations, keeping functionality modular and easy to navigate. 
The client automatically manages API requests, response handling, and pagination where needed, allowing you to focus on 
integrating Monday.com into your workflow without worrying about low-level request details.


A full list of all available methods can be found in the next sections of the documentation.

---

## Return Behavior

The following table outlines the expected return values for different types of methods in the API client.

| **Method Type**                   | **Success Return Value**          | **Failure Return Value**         |
|-----------------------------------|-----------------------------------|--------------------------------|
| **Getters** (Retrieve Data)       | `dict` / `list` of retrieved data | `None` or `response` (error) |
| **Setters** (Create/Update)       | Item UUID                         | `None` or `response` (error) |
| **Delete Methods** (Delete/Clear) | `True` (if deleted successfully)  | `None` or `response` (error) |



---

