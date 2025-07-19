#CMD command we can override 
#ENTRYPOINT cannot be overriden but it will append the command
#But we can use both CMD and ENTRYPOINT combinely for better results where we can override if we don't want default 
#commands to execute
FROM almalinux:9
#CMD ["ping", "google.com"]
#ENTRYPOINT ["ping", "google.com"]
CMD ["google.com"]
ENTRYPOINT ["ping"]