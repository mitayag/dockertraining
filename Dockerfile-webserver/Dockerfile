# Use the official Ubuntu base image
FROM ubuntu:latest

# Update the package list and install Apache
RUN apt-get update && \
    apt-get install -y apache2 && \
    apt-get clean

# Expose port 80 to allow external access to the web server
EXPOSE 80

# Start Apache in the foreground to keep the container running
CMD ["apache2ctl", "-D", "FOREGROUND"]
