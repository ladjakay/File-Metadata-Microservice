# File Metadata Microservice

Upload a file using the form on the home page or send a `multipart/form-data`
`POST` request to `/api/fileanalyse` with the file field named `upfile`.

The API responds with the uploaded file's original name, MIME type, and size in
bytes:

```json
{
  "name": "example.txt",
  "type": "text/plain",
  "size": 12
}
```

Start the service with `npm start`. It listens on port `3000` by default; set
`PORT` to use a different port.
