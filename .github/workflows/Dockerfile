# Use the official Nginx image as base
FROM nginx:alpine

# Maintainer info (optional but good practice)
LABEL maintainer="chandra005 <chandra005@example.com>"

# Remove default nginx page
RUN rm -rf /usr/share/nginx/html/*

# Copy your static website or index.html into the container
COPY ./html /usr/share/nginx/html

# Expose port 80
EXPOSE 80

# Start Nginx (by default the base image already runs nginx)
CMD ["nginx", "-g", "daemon off;"]
