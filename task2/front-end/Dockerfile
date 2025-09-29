# task2/front-end/Dockerfile
FROM nginx:latest

# Copy site files
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy Nginx server config
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

EXPOSE 9000
CMD ["nginx", "-g", "daemon off;"]
