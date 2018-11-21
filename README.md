# Node.js Express Upload Web

This is a tool container for test file upload.

## Run Server

```
docker run -d -p 80:8000i -v /data:/app/uploads peihsinsu/nodejs-express-uploader
```

## Test upload from curl

```
curl -X POST http://localhost:8000/upload -F 'sampleFile=@path/of/your/file'
```

## Test upload from web

Use browser to open: http://your-server-address/form


After upload done, uploaded file will in /app/uploads inside the container. If you mount the folder outside the container, you can find the file there.
