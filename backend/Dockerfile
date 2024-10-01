# backend/Dockerfile

FROM python:3.11.4-slim-buster

# Set the working directory
WORKDIR /django_app

# Copy the requirements file
COPY requirements.txt .

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the code
COPY . .

# Set environment variables (optional)
ENV PYTHONUNBUFFERED 1
