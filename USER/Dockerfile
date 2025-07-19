#USER is to restrict the container for better security and auditability
#So that no other containers can be disturbed or accesssed
FROM almalinux:9
RUN dnf install nginx -y
RUN useradd johnson
USER johnson
CMD ["google.com"]
ENTRYPOINT ["ping"]