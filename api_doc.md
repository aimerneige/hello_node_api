# API Doc

## Login

| request url | request way |
| ----------- | ----------- |
| /login      | POST        |

| Parameter | Required | Description  |
| --------- | -------- | ------------ |
| uid       | MUST     | user account |
| psw       | MUST     | password     |

```json
{
    "status": 200,
    "msg": "Login Success!",
    "token": "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJkYXRhIjoiNWU5MTIwMTViOWI0NmYzZmE4Y2MzMjUzIiwiZXhwIjoxNTg2OTUyMzk1LCJpYXQiOjE1ODY5NTA1OTV9.IsprCaQ_gZRh0BzS8SnAd0iJ27BOpOEb-ZGn0bTlwHVPTiYPK50wiEOL_0aAYINfNT_Mfvb726l3CpiHG9lsJ45m4eqhPeJz9TbAeQj8-ST3CAkYLrD0fhgRG9YiQ5kjVpygdR8NZEWEUV7ux-moyYe7wCoVzN9mbvAkFF3IYG0"
}
```

## POST data

| request url | request way |
| ----------- | ----------- |
| /data/new   | POST        |

| Parameter | Required | Description |
| --------- | -------- | ----------- |
| token     | MUST     | User token  |
| info      | MUST     | Information |

```json
{
    "status": 200,
    "msg": "Create Success!",
    "id": "100001"
}
```

## GET data

| request url | request way |
| ----------- | ----------- |
| /data/cat/  | GET         |

| Parameter | Required | Description |
| --------- | -------- | ----------- |
| token     | MUST     | User token  |
| id        | MUST     | Data id     |

```json
{
    "status": 200,
    "msg": "Get Data Success!",
    "info": "Some useful information."
}
```

## EDIT data

| request url | request way |
| ----------- | ----------- |
| /data/edit  | POST        |


| Parameter | Required | Description     |
| --------- | -------- | --------------- |
| token     | MUST     | User token      |
| id        | MUST     | Data id         |
| new       | MUST     | New Information |

```json
{
    "status": 200,
    "msg": "Edit Data Success!"
}
```