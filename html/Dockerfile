# Use official Nginx image
FROM nginx:alpine

# Remove default Nginx website
RUN rm -rf /usr/share/nginx/html/*

# Copy static HTML content
COPY . /usr/share/nginx/html

# Expose default HTTP port
EXPOSE 80
