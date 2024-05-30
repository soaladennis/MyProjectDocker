# Use an official Nginx runtime as a parent image
FROM nginx:stable-alpine

# Remove the default Nginx configuration
RUN rm -rf /usr/share/nginx/html/*

# Copy the application files to the Nginx HTML directory
COPY . /usr/share/nginx/html

# Expose port 80 for incoming HTTP traffic
EXPOSE 80

# Start Nginx when the container launches
CMD ["nginx", "-g", "daemon off;"]