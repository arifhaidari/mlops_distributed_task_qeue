# Distributed Task (Under Development)

### Tools used in the project:

first start from building the core logic and then integrate the other piece later.
for example start with developing the models first and then the core logic which
could be runs manually and then start automating things and then notifications and other
sophisticated things

A microservices-based system
FastApi (if it is a recommendation system using my old e-commerce websites) this can be a reccomendation with movies as well since the data will be widely available

Docker
Docker Compose
Redis
Celery
Flower
Beat
MLFlow

Alertmanager is used to send alerts (via email, Slack, or other platforms) when something goes wrong in your Kubernetes cluster.

Loki
log collection. Centralized log collection for Celery, FastAPI, and MLflow

Prometheus (why needed and other alternative)
Monitor system metrics (CPU, RAM) and Celery tasks
it is monitoring and alerting toolkit
Real-world use case:
Imagine you run an e-commerce website. Prometheus can monitor key metrics like:
Server CPU and memory usage.
Application response times.
Number of failed transactions.
API request rates.

Grafana (why needed and other alternatives)
Visualize logs & metrics
visualization and analytics platform. create dashboards and graphs for time-series data, logs, and other metrics.

Kafka (why need and other alternatives)
database: mongodb

Kubernetes (do I need it)
dev environment, staging environment, and production environment

Elasticsearch (do I need it)

Helm:
How They Work Together
Kubernetes provides the underlying infrastructure to run containers.
Helm packages the application (e.g., frontend, backend, database) into a Chart and deploys it to Kubernetes.
Helm uses Kubernetes manifests (e.g., Deployments, Services) under the hood but adds a layer of abstraction for easier management.
Kubernetes is the foundation for running containerized applications.
Helm is a tool built on top of Kubernetes to simplify application deployment and management.
Think of Kubernetes as the engine that runs your applications and Helm as the driver that makes it easier to operate the engine. Together, they provide a powerful platform for deploying and managing modern applications.

OpenTelemetry for Better Tracing
To enhance observability, we'll integrate OpenTelemetry with our distributed MLOps system. This will allow us to trace requests across services (FastAPI, Celery, and RabbitMQ) and monitor latency, errors, and bottlenecks.

all of the above will be used in a Distributed system

Deployment:
Deploying the Distributed MLOps System to AWS EKS
Now, we will move our Kubernetes-based distributed MLOps system to AWS Elastic Kubernetes Service (EKS).

---

Message Broker
In-memory Key-Value Store & Message Broker
Beat will schedule scrapers - Task Scheduler
Elasticsearch

### potential project:

book recommender system

movie recommender system

and my ecommerce website

or all of them (at least for model development and then decide which one to continue)

Or:
we use the breast cancer project to apply all the MLOPs principle while it is easier to collect data and do the inference and there is no for historical data. but the goal is to have MLOPs applied.

and create three projects with recommendation:
book, movie and other goods (explore using LLMs)
