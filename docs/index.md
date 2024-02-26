# Overview

PyMonday is a monday.com API Python Client Library, compatible with API version 2023-10 and later.

### Official API Documentation

<a href='https://developer.monday.com/api-reference/docs/basics'>Monday API Documentation</a>

### Installation

To install pymonday, use the following pip command in your project virtual environment.

```bash
pip install pymonday
```

### API Authentication

You must pass your monday.com API key to the MondayAPIClient object to authenticate API calls.

Review the Official API Documentation for instructions on obtaining an API Key. 

### Instantiate Client Object

To import the monday.com API client into your project, use the following import statement:
```python
from pymonday import MondayAPIClient
```

An instance of the API Client Object can then be created:
```python
monday = MondayAPIClient(api_key="API_KEY")
```

The object can then be called and its methods accessed in order to interact with the monday.com API:

Example:
```monday.get_user_info(user_id=12345)```

A full list of all available methods can be found in the next sections of the documentation.

---

