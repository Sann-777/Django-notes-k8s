# 🧠 Django Notes App | Deployed with Kubernetes on AWS

## 🚀 About the Deployment

I wanted to take a hands-on approach to learning Kubernetes, so I decided to deploy a Django Notes app using `kind` (Kubernetes in Docker) and expose it publicly from an AWS EC2 instance. Here's what I did:

- 🔧 Set up a local Kubernetes cluster using `kind`
- 🐳 Uploaded the Docker image to Docker Hub
- 🗂️ Created a namespace to logically group the container, pod, deployment, and service
- 📄 Used `deployment.yaml` to create a pod and run the app inside the container
- 🌐 Exposed the app internally using a Kubernetes `service.yaml` file
- 📡 Used port forwarding to bind the container port to the EC2 host port, making it accessible to the public


---

## ⚙️ Tech Stack for Deployment

- **Docker** (Containerization)
- **Kubernetes** (Orchestration)
- **kind** (Local K8s cluster)
- **AWS EC2** (Cloud host)
- **YAML** (K8s configurations)

---

## ✨ What I Learned

This wasn’t just about getting it to work — I got to understand:
- How containers run inside pods and how deployments work
- The relationship between services and port-forwarding
- Exposing apps on the internet through EC2 and Kubernetes
- Debugging services and pods when things don’t go as expected 😅

This project was a great learning experience and gave me real confidence working with K8s beyond tutorials.

---

## 📄 Kubernetes YAML Files

The core Kubernetes configurations used to deploy the app are in k8s folder


