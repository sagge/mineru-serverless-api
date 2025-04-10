# PDF parsing API based on MinerU

- MinerU GPU Image Construction
- PDF parsing interface based on FastAPI

## Build method

```
docker build -t mineru-api .
```

Or use a proxy:

```
docker build --build-arg http_proxy=http://127.0.0.1:7890 --build-arg https_proxy=http://127.0.0.1:7890 -t mineru-api .
```

## Startup Command

```
docker run --rm -it --platform=linux/amd64 --gpus=all -p 8000:8000 mineru-api
```

## Test Parameters

Visit URL:

```
http://localhost:8000/docs
http://127.0.0.1:8000/docs
```