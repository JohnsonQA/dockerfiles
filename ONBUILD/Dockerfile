#Onbuild is used for the users who use the other image where which we have to make it mandate to have a specific file
#Eg. In below index.html is mandate for nginx. So we removing in our container and making it mandate so that others
#use it by having their own index.html


#Nutsehll, If someone build their docker image from mine then I am settingup a restriction saying hey if u wanna
# use my image then u must have index.html in ur image to use mine. 
# Purporse of it is for users to add specific files
#Great when sharing base images with team

FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ONBUILD copy index.html /usr/share/nginx/html/index.html
CMD ["nginx", "-g", "daemon off;"]