# E-Commerce Microservices

Microservices architecture for e-commerce with Kafka event streaming.

## 🚀 Quick Start

### Prerequisites
- Docker Desktop installed
- Docker Compose installed

### Run Everything

```bash
# Clone the repository
git clone <your-repo-url>
cd E-commerce-microservice

# Start all services
docker-compose up -d --build

# View logs
docker-compose logs -f
```

### Access Services
- **Frontend**: http://localhost:3000
- **Payment API**: http://localhost:8000
- **Kafka UI**: http://localhost:8080

### Stop Services
```bash
docker-compose down
```

## 📦 Services

- **Payment Service** (Port 8000) - Handles payments
- **Order Service** - Processes orders
- **Email Service** - Sends notifications
- **Analytics Service** - Collects metrics
- **Client** (Port 3000) - Next.js frontend
- **Kafka Cluster** - 3 brokers for event streaming

## 🏗️ Architecture

```
Client (Next.js) → Payment Service → Kafka → Order/Email/Analytics Services
```