#CMD instruction is about start the services or do some actions on those services
#It basically runs at the time of container creation means during docker run or docuker build
# Should be only one CMD instruction inside docker file
#CMD [] is nothing but systemctl start nginx. Since systemctl runs on kernel we directly use it
# where as docker cannot be run on kernel so we should follow as below

FROM run:v1
CMD ["nginx", "-g", "daemon off;"]