# Easy-Order Staff App API Documentation 

## Error Response
```json
{
    "code": "error_code",
    "detail": "Error message."
} 
```

---
## Customer List
* **Endpoint:** _/api/customer/_
* **Method:**   _GET_
* **Headers:** 
    ```json
    {
        "Authorization" : "Bearer thisIsASampleTokenOnlyDoNotCopy"
    } 
    ```
* **Parameters:**
    ```json
    none
    ```
* **Response:**
    ```json
    [{
        "id": 113,
        "user": {
            "id": 115,
            "password": "pbkdf2_=",
            "last_login": null,
            "is_superuser": false,
            "username": "otameshicustomer74",
            "first_name": "Taro",
            "last_name": "Yamada",
            "email": "admin@admin.com",
            "is_staff": false,
            "is_active": true,
            "date_joined": "2019-01-23T13:27:59.481572+09:00",
            "groups": [],
            "user_permissions": []
        },
        "created": "2019-01-23T13:27:59.514082+09:00",
        "modified": "2019-01-23T13:27:59.518998+09:00",
        "is_removed": false,
        "first_name_chinese": "太郎",
        "last_name_chinese": "山田",
        "phone_number": null,
        "code": "001",
        "customer_code": "",
        "device": false,
        "store": 74,
        "role": 6
    }]
    ```





---
## Customer Modify
* **Endpoint:** _/api/customer/_
* **Method:**   _PUT_
* **Headers:** 
    ```json
    {
        "Authorization" : "Bearer thisIsASampleTokenOnlyDoNotCopy"
    } 
    ```
* **Parameters:**
    ```json
    {
        "id": 113
    }
    ```
* **Response:**
    ```json
    {
        "code": "success",
        "detail": "Successfully modified."
    }
    ```
    > Same structure of Error response.




---
## Customer Delete
* **Endpoint:** _/api/customer/_
* **Method:**   _Delete_
* **Headers:** 
    ```json
    {
        "Authorization" : "Bearer thisIsASampleTokenOnlyDoNotCopy"
    } 
    ```
* **Parameters:**
    ```json
    {
        "id": 113
    }
    ```
* **Response:**
    ```json
    {
        "code": "success",
        "detail": "Successfully deleted."
    }
    ```
    > Same structure of Error response.




## Customer Add
* **Endpoint:** _/api/customer/_
* **Method:**   _POST_
* **Headers:** 
    ```json
    {
        "Authorization" : "Bearer thisIsASampleTokenOnlyDoNotCopy"
    } 
    ```
* **Parameters:**
    ```json
    {
        "first_name": "Tristan",
        "last_name": "Galang",
        "first_name_chinese": null,
        "last_name_chinese": null,
        "email": "tac.galang@gmail.com",
        "username": "tristan",
        "password": "1234",
        "customer_code":"123"
    }
    ```
* **Response:**
    ```json
    {
        "code": "success",
        "detail": "Successfully added."
    }
    ```
    > Same structure of Error response.
