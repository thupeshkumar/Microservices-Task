cd Microservices-Task
echo "# Microservices Containerization Assessment

## 📌 Project Overview
This project demonstrates containerization of **Node.js microservices** using **Docker** and **Docker Compose**.  
The application consists of the following services, each running in its own container and communicating via a shared Docker network:

- **User Service**
- **Product Service**
- **Order Service**
- **Gateway Service**

--- 

## 📂 Project Structure
\`\`\`
Microservices-Task/
│
├── Microservices/
│   ├── user-service/
│   │   └── Dockerfile
│   ├── product-service/
│   │   └── Dockerfile
│   ├── order-service/
│   │   └── Dockerfile
│   └── gateway-service/
│       └── Dockerfile
│
├── docker-compose.yml
└── README.md
\`\`\`

--- 

## ⚙️ Prerequisites
Ensure the following software is installed:
- Docker
- Docker Compose
- Git

--- 

## 🚀 Setup Instructions

### Step 1: Clone Repository
\`\`\`bash
git clone https://github.com/thupeshkumar/Microservices-Task.git
cd Microservices-Task
\`\`\`

### Step 2: Build & Run Containers
\`\`\`bash
docker compose -f Microservices/docker-compose.yml up -d --build
\`\`\`

✅ This will build images and start all services in detached mode.

--- 

## 🔌 Services and Ports
| Service          | Port |
|------------------|------|
| User Service     | 3000 |
| Product Service  | 3001 |
| Order Service    | 3002 |
| Gateway Service  | 3003 |

--- 

## 📡 API Testing

### User Service
- GET /users → Fetch all users

### Product Service
- GET /products → Fetch all products

### Order Service
- GET /orders → Fetch all orders

### Gateway Service
- GET /gateway/users → Fetch users via gateway  
- GET /gateway/products → Fetch products via gateway  
- GET /gateway/orders → Fetch orders via gateway  

--- 

## 🛠️ Docker Compose Features
- Multi-container orchestration  
- Shared networking  
- Port mapping  
- Service dependency management  

--- 

## 🧩 Troubleshooting

### Port Already in Use
Check running containers:
\`\`\`bash
docker ps
\`\`\`
Stop containers if necessary:
\`\`\`bash
docker compose down
\`\`\`

### View Logs
\`\`\`bash
docker logs user-service
\`\`\`

--- 

## ✅ Conclusion
All microservices were successfully containerized using Docker and orchestrated with Docker Compose.  
They communicate seamlessly over a shared Docker network and are accessible via their respective ports." > README.md
