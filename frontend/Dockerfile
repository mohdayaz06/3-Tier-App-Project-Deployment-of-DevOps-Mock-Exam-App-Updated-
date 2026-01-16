# Use a lightweight web server image
FROM nginx:alpine

# Remove default nginx static assets
RUN rm -rf /usr/share/nginx/html/*

# Copy only the HTML files into the nginx html folder
COPY *.html /usr/share/nginx/html/

# Ensure the nginx user can read the files
RUN chmod -R 755 /usr/share/nginx/html

# Expose port 80
EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
