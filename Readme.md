# User API Specification

## Create User
Endpoint : POST /api/users

Request Body :

```json
{
  "nama" : "Linda",
  "usia" : 20
}
```

Response Body (success) :

```json
{
  "data": {
    "id" : "random string",
    "nama": "Linda",
    "usia": 20
  }
}
```

Response Body (failed) :

```json
{
  "error": "Invalid input data"
}
```

## Update User
Endpoint : PUT /api/users/{id}

Request Body :

```json
{
  "nama" : "Linda",
  "usia" : 19
}
```

Response Body (success) :

```json
{
  "data": {
    "id" : "random string",
    "nama": "Linda",
    "usia": 19
  }
}
```

Response Body (failed) :

```json
{
  "error": "User not found"
}
```

## Get User
Endpoint : GET /api/users

Response Body (success) :

```json
{
  "data": {
    "id" : "random string",
    "nama": "Linda",
    "usia": 19
  }
}
```

Response Body (failed) :

```json
{
  "error": "User not found"
}
```

## Delete User
Endpoint : DELETE /api/users/{id}

Response Body (success) :

```json
{
  "message": "User deleted successfully"
}
```

Response Body (failed) :

```json
{
  "error": "User not found"
}
```