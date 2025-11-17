# Deployment Guide

## 1. Build using Maven
mvn clean package

## 2. Build Docker Image
docker build -t tms-backend .

## 3. Run Docker Container
docker run -p 8080:8080 tms-backend

## 4. Push Image to GitHub Container Registry
docker tag tms-backend ghcr.io/YOUR-USERNAME/tms-backend:latest
docker push ghcr.io/YOUR-USERNAME/tms-backend:latest
