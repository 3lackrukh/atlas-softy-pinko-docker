# Host from nginx web-server
FROM nginx:latest

# Copy config file to nginx config folder as default
COPY ./proxy.conf /etc/nginx/conf.d/default.conf

# Open port 80 for incoming requests
EXPOSE 80