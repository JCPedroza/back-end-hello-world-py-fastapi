# Python Back-End Hello World: FastAPI

Write a Python program that listens to `localhost:8000` and responds
with the json `{ "hello": "world" }` to a `get` request directed at the
root endpoint located at `/`.

## Install needed packages

```bash
pip install fastapi uvicorn
```

## Start server and run app

```bash
uvicorn main:app
```

## Send get request to root

```bash
http localhost:8000 # using httpie in debian
```

Should return header and body similar to:

```text
HTTP/1.1 200 OK
content-length: 17
content-type: application/json
date: Fri, 14 Feb 2024 05:29:06 GMT
server: uvicorn

{
    "hello": "world"
}
```
