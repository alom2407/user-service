
# User Service

user service can used to authenticate the user or onboard a new user on your platform. It uses PKI to sign and create the token. Those token can be used to authenticate api requests. 

## Flow Diagram

## API Reference

#### Get all user details 

```http
  GET /users/
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `token` | `string` | **Required**.  authentication token |

#### Get user details of yourself

```http
  GET /users/me
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `token`      | `string` | **Required**. authentication token |

#### Post Signup New User

```http
  POST /auth/signup
```

Signup a new user on platform

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `email`      | `string` | **Required**.
| `password`      | `string` | **Required**.
| `firstName`      | `string` | **Required**. 

#### Post User Login

```http
  POST /auth/login
```

User login on platform

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `email`      | `string` | **Required**.
| `password`      | `string` | **Required**.



## Tech Stack

**Server:** Java, Springboot, Spring Security, Maven, Rest API, JWT, PKI, database(mySQL/postgres/noSQL)



## Authors

- [@Alom Jaiswal](https://github.com/alom2407)

