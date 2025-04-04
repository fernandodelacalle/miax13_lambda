# miax13_lambda

Construir la imagen:
```bash
docker build -t 076977333390.dkr.ecr.eu-west-1.amazonaws.com/miax13_lambda .
```

Si la quiero probar:
```bash
docker run -p 9000:8080 076977333390.dkr.ecr.eu-west-1.amazonaws.com/miax13_lambda
curl -XPOST "http://localhost:9000/2015-03-31/functions/function/invocations" -d '{}'
```

Subir la imagen al ECR
```bash
docker push 076977333390.dkr.ecr.eu-west-1.amazonaws.com/miax13_lambda
```