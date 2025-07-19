#USER is to restrict the container for better security and auditability
#So that no other containers can be disturbed or accesssed
#It will keep the container running as normal user/non-root user
FROM almalinux:9
RUN dnf install nginx -y
RUN useradd johnson
USER johnson
CMD ["google.com"]
ENTRYPOINT ["ping"]