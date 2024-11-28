# Use an official Python runtime as a parent image
FROM python:3.9-slim

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents (the src folder) into the container at /app
COPY . /app/

# Copy the requirements.txt from the parent folder to the container
COPY ../requirements.txt /app/requirements.txt

# Install any dependencies specified in requirements.txt
RUN pip install --no-cache-dir -r /app/requirements.txt

# Expose the port (if using Flask)
EXPOSE 5000

# Run app.py when the container launches
CMD ["python", "app.py"]
