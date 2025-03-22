# Use the official Python image from the Docker Hub
FROM python:3.12.1

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir --upgrade pip && \
    pip install --no-cache-dir -r requirements.txt

# Make port 80 available to the world outside this container
EXPOSE 80 8001

# Define environment variable
ENV PYTHONUNBUFFERED=1

# Run the application
CMD ["python", "/app/app/main.py"]