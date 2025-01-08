# Use a base Python image
FROM python:3.9-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the requirements.txt (Python dependencies) into the container
COPY requirements.txt .

# Install the dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the application files into the container
COPY . .

# Expose the port the app runs on (adjust if using a different port)
EXPOSE 8000

# Set the default command to run the server (adjust based on your app's entry point)
CMD ["python", "server.py"]
