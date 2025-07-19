#workdir is used to set up a working directory for the container
FROM almalinux:9
RUN mkdir /tmp/workdir-demo
#RUN cd /tmp/workdir-demo  cd won't switch to directory so is workdir we use
WORKDIR /tmp/workdir-demo
RUN pwd
RUN echo "Hello I am in work dir" > hello.txt
CMD ["sleep","1000"]