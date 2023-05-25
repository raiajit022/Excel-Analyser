# Use Python 3.9 slim image as base
FROM python:3.9-slim-buster

# Set the working directory to /app
WORKDIR /app

# Copy app files and requirements.txt to /app
COPY . .

# Install required Python packages
RUN pip install --no-cache-dir -r requirements.txt

# Expose port 8501
EXPOSE 8501

# Run Streamlit app
CMD ["streamlit", "run", "app.py", "--server.port", "8501", "--server.address", "0.0.0.0"]

#To build a Docker image from this Dockerfile, you can use this command:
 #docker build -t streamlit-app# .
#To run the Docker image, you can use this command:
    #docker run -p 8501:8501 streamlit-app
