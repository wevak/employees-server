## Introduction
This is an employee record keeping application storing employee's name, position and level while having basic crud features.

```http
GET /record
```
| Parameter | Type | Description | Curl |
| :--- | :--- | :--- | :--- |
| `none` |  | Enlists list of all employees| curl -s https://employees-server-l554.onrender.com/record  |

```http
POST /record
```
| Parameter | Type | Description | Curl |
| :--- | :--- | :--- |  :--- |
| `HTTP body` | `User Object` | To create employee record |curl -X POST -H "Content-Type: application/json" -d "{ \"name\": \"test5\", \"position\": \"test5\", \"level\": \"test5\" }" https://employees-server-l554.onrender.com/record|

```http
GET /record/:_id
```
| Parameter | Type | Description | Curl |
| :--- | :--- | :--- | :--- |
| `/id` | `String` | To fetch certain employee | curl -s https://employees-server-l554.onrender.com/record/66b8be9dc4deec0304af810f |

```http
DELETE /record/:_id
```
| Parameter | Type | Description | Curl |
| :--- | :--- | :--- | :--- |
| `/id` | `String` | To delete a certain employee record | curl -X DELETE -H "Content-Type: application/json" https://employees-server-l554.onrender.com/record/66eaaa64d7703edcbdeacde4|

```http
PATCH /record/:_id
```
| Parameter | Type | Description | Curl |
| :--- | :--- | :--- | :--- |
| `/id` | `String` | To update a certain employee record| curl -X PATCH -H "Content-Type: application/json" -d "{ \"name\": \"test4\", \"position\": \"test4\", \"level\": \"test4\" }" https://employees-server-l554.onrender.com/record/66c82ce80f7c90f0e42697e8|