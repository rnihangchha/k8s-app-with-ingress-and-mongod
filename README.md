## Project Structure

```
my-kubernetes-app/
├── app-svc.yaml
├── app.yaml
├── ingress.yaml
├── db/
│   ├── mongo-config.yaml
│   ├── mongo-headless-svc.yaml
│   ├── mongo-secret.yaml
│   ├── mongo-service.yaml
│   └── mongo.yaml
├── pv1.yaml
├── pv.yaml
└── flask-apps/
    ├── app.py
    ├── Dockerfile
    ├── requirements.txt
    └── templates/
        └── index.html
```
