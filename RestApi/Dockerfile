# Use the official Python Alpine base image
FROM python:3.9-alpine

# Set the working directory in the container
WORKDIR /app

# Copy the requirements file
COPY requirements.txt .

# Install the dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the Flask application code into the container
COPY app.py .

# Expose the port that the Flask application will run on
EXPOSE 5000

# Set the command to run the Flask application using Gunicorn
#testing
CMD ["gunicorn", "--bind", "0.0.0.0:5000", "app:app"]
