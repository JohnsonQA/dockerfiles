#Copy will copy local files into container
FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
COPY index.html /usr/share/nginx/html/
CMD ["nginx", "-g", "daemon off;"]