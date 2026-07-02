Requirement

↓

Design

↓

Documentation

↓

Development

↓

Testing

↓

Deployment



* High-Level Architecture (HLD)
React

                   │

             API Gateway

                   │

     ┌─────────────┼─────────────┐

Auth      Patient      Doctor

     │             │              │

Appointment     Billing      AI


* Low-Level Design (LLD)
Auth Service contains:
1. User
2. Role
3. JWT
4. Security
5. Controller
6. Service
7. Repository

* Database Design
patient_id

first_name

last_name

dob

blood_group



* Microservice Communication

Patient Service

↓

Appointment Service

↓

Kafka

↓

Notification Service


* Security Architecture
User

↓

Login

↓

JWT

↓

Gateway

↓

Patient Service

* Kafka Events
AppointmentCreated

BillGenerated

PrescriptionCreated

PaymentCompleted

* Redis
Doctor Availability

↓

Redis

↓

Avoid Database Call

* AI Architecture ⭐
PDF Upload

↓

Chunking

↓

Embeddings

↓

Vector Database

↓

LLM

↓

Answer

* Deployment Guide
  docker-compose up
