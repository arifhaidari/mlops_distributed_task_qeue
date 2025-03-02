# Distributed Task (Under Development)

### Tools used in the project:

Docker
Redis
Celery

---

Message Broker
In-memory Key-Value Store & Message Broker
Beat will schedule scrapers - Task Scheduler
Elasticsearch

### Project Draft Idea

Distributed Image Processing System
Idea: Upload images, process them (resize, grayscale, etc.), and return the processed image.
Tools: Celery + RabbitMQ + Redis + Flower
Why? Celery will distribute tasks across workers, RabbitMQ will queue requests, Redis will cache processed images, and Flower will help monitor workers.
