# Use Nginx web-server to host
FROM nginx:latest

# Copy front end folder to image
COPY ./softy-pinko-front-end /usr/www/html/softy-pinko-front-end

# Copy and rename config file to default location in image
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# Open port 9000 for app to listen
EXPOSE 9000