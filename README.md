# 🍕 Cloud Pizza Factory - Docker & Kubernetes Mini Project

## 📌 Project Overview

Cloud Pizza Factory is a simple Flask web application packaged with Docker and deployed using Kubernetes. The project demonstrates how containerization and orchestration work together to build scalable and highly available applications.

This project is designed for beginners to understand the concepts of Docker, Containers, Docker Images, Kubernetes Pods, Deployments, and Scaling.

---

## 🎯 Objective

- Build a simple Python web application.
- Package the application using Docker.
- Run the application inside a Docker container.
- Deploy the container using Kubernetes.
- Scale the application with multiple replicas.
- Demonstrate Kubernetes self-healing by recreating failed pods.

---

## 🛠️ Technologies Used

- Python 3.11
- Flask
- Docker
- Kubernetes
- kubectl

---

## 📂 Project Structure

```
cloud-pizza/
│── app.py
│── requirements.txt
│── Dockerfile
│── deployment.yaml
└── README.md
```

---

## ⚙️ How It Works

1. A Flask application displays the Cloud Pizza Factory homepage.
2. Docker packages the application along with all dependencies.
3. A Docker image is created.
4. Docker runs the application inside a container.
5. Kubernetes deploys multiple container replicas.
6. If a container fails, Kubernetes automatically creates a new one.
7. The application can be scaled up or down based on traffic.

---

## 🚀 Installation

### Clone Repository

```bash
git clone https://github.com/your-username/cloud-pizza-factory.git

cd cloud-pizza-factory
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Run Application

```bash
python app.py
```

Open:

```
http://localhost:5000
```

---

## 🐳 Docker Commands

### Build Docker Image

```bash
docker build -t cloud-pizza .
```

### Run Docker Container

```bash
docker run -p 5000:5000 cloud-pizza
```

Application will be available at:

```
http://localhost:5000
```

---

## ☸️ Kubernetes Deployment

Deploy the application:

```bash
kubectl apply -f deployment.yaml
```

Check running pods:

```bash
kubectl get pods
```

Check deployment:

```bash
kubectl get deployments
```

---

## 📈 Scaling the Application

Increase replicas:

```bash
kubectl scale deployment cloud-pizza --replicas=5
```

Decrease replicas:

```bash
kubectl scale deployment cloud-pizza --replicas=1
```

---

## 🔄 Self-Healing Demonstration

Delete a pod:

```bash
kubectl delete pod <pod-name>
```

Kubernetes automatically creates a new pod to maintain the desired number of replicas.

---

## 📸 Expected Output

Home Page:

```
🍕 Welcome to Cloud Pizza Factory

Today's Special:
Paneer Tikka Pizza
```

After Kubernetes deployment:

- Multiple Pods running
- Automatic pod recovery
- Easy scaling
- High Availability

---

## 📚 Key Concepts Learned

- Docker Image
- Docker Container
- Dockerfile
- Kubernetes
- Pod
- Deployment
- Replica
- Scaling
- Self-Healing
- Container Orchestration

---

## 🎯 Future Enhancements

- Add Kubernetes Service
- Use ConfigMaps
- Store configuration in Secrets
- Deploy on AWS EKS
- Add CI/CD using GitHub Actions
- Monitor application using Prometheus and Grafana

---

## 👩‍💻 Author

**Neha Balkawade**

---

## ⭐ If you found this project useful, don't forget to star the repository!
