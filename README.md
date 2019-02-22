# PetiteURL

A URL shortening service in Node.js

## Demo

![](demo.gif)

## Getting Started

```
$ npm install
```

Create a file `.env` and specify environment variable(s)

Start a MongoDB instance:

```
$ sudo mongod
```

For example:
`DATABASE=mongodb://localhost:27017`

Run in development environment:

```
$ npm run dev
```

Run in production environment:

```
$ npm run start
```

## Endpoints:

### Create new short_url

`POST /new`

Example request body:

```json
{
  "url": "https://www.youtube.com/"
}
```

Response:

```json
{
  "original_url": "https://www.youtube.com/",
  "short_id": "-f_vN1V"
}
```
