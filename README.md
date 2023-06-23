
# 👋Wavy

This repository is the parent repository of the Wavy project. Frontend and Backend are linked as submodules.

**👋 Wavy** is a RSVP app for any kind of event with a very simple interface making it simple and fun.


## Tech Stack

**Client:** React,  TailwindCSS

**Server:** Node, Express


## Deployment

The project is deployed at netlify

```bash
  https://wavy-rsvp.netlify.app/
```


## API Reference

### Auth Routes

#### To login

```http
  POST /api/auth/login
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `email` | `string` | **Required**. Your Email ID |
| `password` | `string` | **Required**. Your password |

**The project uses bcrypt based hashing so password is safe.**

#### Register a user

```http
  POST /api/auth/register
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `email` | `string` | **Required**. Your Email ID |
| `password` | `string` | **Required**. Your password |

### Event Routes

#### Create a new event

```http
  POST /api/event/create
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `userId` | `ObjectID` | **Required**. Parent user's uuid |
| `name` | `string` | **Required**. Event's name |



#### Register in an event

```http
  POST /api/auth/register
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `useremail` | `string` | **Required**. User's email |
| `eventname` | `string` | **Required**. Event's name |




## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`MONGODB_CONNNECTION_STRING`

`PORT`


## Run Locally

Clone the project

```bash
  git clone https://github.com/tusharbansal22/Wavy-frontend
```

Go to the project directory

```bash
  cd Wavy-frontend
```

Install dependencies

```bash
  npm i
```

Start the client

```bash
  npm start
```

Clone the project

```bash
  git clone https://github.com/tusharbansal22/Wavy-backend
```

Go to the project directory

```bash
  cd Wavy-backend
```

Install dependencies

```bash
  npm i
```

Start the server

```bash
  nodemon server.js
```


## Contributing

Contributions are always welcome!

See `contributing.md` for ways to get started.

Please adhere to this project's `code of conduct`.

