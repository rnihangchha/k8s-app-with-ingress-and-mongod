 A containerized Flask web framework deployed as a Kubernetes Deployment and a persistent MongoDB database managed as a StatefulSet,
 all running on a Minikube cluster. External user traffic is routed through an Ingress resource defined with path-based rules, 
 which is provisioned and managed by the NGINX Ingress Controller; this controller itself is exposed via a LoadBalancer service,
 providing the public entry point to access the web application seamlessly.

├── app
│   ├── app-svc.yaml
│   ├── app.yaml
│   └── ingress.yaml
├── db
│   ├── mongo-config.yaml
│   ├── mongo-headless-svc.yaml
│   ├── mongo-secret.yaml
│   ├── mongo-service.yaml
│   ├── mongo.yaml
│   ├── pv1.yaml
│   └── pv.yaml
└── flask-apps
    ├── app.py
    ├── Dockerfile
    ├── requirement.txt
    └── templates
        └── index.html

5 directories, 14 files
