# Use the official Ubuntu image as a base
FROM ubuntu:latest

# Update and install required packages
RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y python3 python3-pip

# Remove externally managed flag
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask using pip
RUN pip3 install flask

# Set the working directory
WORKDIR /app

# Copy the Python file to the container
COPY ./api.py /app/api.py

# Expose the port Flask will run on
EXPOSE 5252

# Command to run the Flask app
CMD ["python3", "api.py"]
