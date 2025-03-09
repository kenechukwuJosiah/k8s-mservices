# k8s-demo

This project is a demonstration of Kubernetes deployment and management.

## Prerequisites

- Docker
- Kubernetes (Minikube or a Kubernetes cluster)
- kubectl

## Setup

1. **Clone the repository:**

```sh
git clone https://github.com/kenechukuJosiah/k8s-demo.git
cd k8s-demo
```

2. **Build the Docker image:**

```sh
docker build -t yourusername/k8s-demo:latest .
```

3. **Deploy to Kubernetes:**

```sh
kubectl apply -f nginx.yml -f hello-service-2-nginx.yml
```

## Usage

- **Check the status of the pods:**

  ```sh
  kubectl get pods
  ```

- **Access the application:**
  ```sh
  minikube service <serviceName>
  ```

## Cleanup

To remove the deployment, run:

```sh
kubectl delete -f nginx.yml -f hello-service-2-nginx.yml
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License.
