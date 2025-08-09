# Fault-Tolerant and Scalable Distributed Job Scheduler

## Description:
This project is an implementation of a distributed job scheduler designed to process tasks efficiently and reliably across a cluster of worker nodes. It showcases core distributed systems concepts such as fault tolerance, load balancing, and inter-process communication. The scheduler uses a central queue to manage tasks and monitors the health of its workers, ensuring that no task is lost even if a worker fails.

---

## Features:

**Task Queuing:** A centralized queue (e.g., using Redis) to store and manage incoming jobs.

**Worker Pool:** A pool of worker nodes that can pull tasks from the queue and execute them in parallel.

**Load Balancing:** An intelligent load balancing algorithm to distribute jobs evenly among available workers.

**Fault Tolerance:** A heartbeat mechanism to detect failed workers and automatically reassign their tasks to other healthy nodes.

**Monitoring:** A simple interface or logging system to track the status of jobs and the health of the worker nodes.

**Scalability:** The system is designed to scale horizontally by simply adding more worker nodes.

---

## Tech Stack:

**Programming Language:** Python

**Queueing System:** Redis

**Communication:** Sockets or a messaging library

**Monitoring:** Custom logging

---

## Installation:

**Clone the repository:**
```bash
git clone [repository_url]
```
**Navigate to the project directory:**
```bash
cd [project_name]
```
**Start the Redis server:**
```bash
redis-server
```
**Run the scheduler:**
```bash
python scheduler.py
```
**Run the workers:**
```bash
python worker.py (you can run multiple instances for a distributed setup).
```
