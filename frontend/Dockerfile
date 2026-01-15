# Use a lightweight web server image
FROM nginx:alpine

# Copy all frontend files into the nginx html folder
COPY . /usr/share/nginx/html

# Expose port 80
EXPOSE 80

# Start nginx server
CMD ["nginx", "-g", "daemon off;"]


