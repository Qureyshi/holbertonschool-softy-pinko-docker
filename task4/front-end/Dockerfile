# Use the official Nginx image as a base
FROM nginx:latest

# Copy front-end files to the Nginx directory
COPY softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy custom Nginx configuration
COPY softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# Expose port 9000
EXPOSE 9000
