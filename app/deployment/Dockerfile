# Use an official Python runtime as a parent image
FROM --platform=linux/amd64 python:3.10.14-slim

# Set the working directory in the container
WORKDIR /app

# Install any needed packages specified in requirements.txt
COPY ./requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy the current directory contents into the container at /app
COPY ./saved_model /app/saved_model
COPY ./main.py /app/main.py

# Run app.py when the container launches
ENTRYPOINT ["python", "-m", "main"] 

