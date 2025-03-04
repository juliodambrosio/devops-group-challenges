FROM nginx:latest

WORKDIR /app

COPY nginx.conf /etc/nginx/nginx.conf

COPY index.html /app/html/

RUN chown -R nginx:nginx /app/html

EXPOSE 80 443

ENTRYPOINT ["nginx", "-g", "daemon off;"]
