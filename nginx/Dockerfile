# Datei: security/nginx/Dockerfile (docbuc/nginx:nonroot)
FROM nginx:alpine

COPY default.conf /etc/nginx/conf.d/
RUN touch /var/run/nginx.pid && \
  chown -R nginx:nginx /var/run/nginx.pid
EXPOSE 8080
USER nginx
