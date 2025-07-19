#workdir is used to set up a working directory for the container so that any actions or configuartions to be on 
#the same dir. Then we can use WORKDIR. CD won't work

#cd won't work cuz each run command runs in seperate shell
# cd /tmp chnages to temp dir and exits
#The next pwd runs in a new shell starting from default / not /tmp
#so thats why we go for WORKDIR

#In short CD is juz for temp change and workdir is permamnent change
FROM almalinux:9
RUN mkdir /tmp/workdir-demo
#RUN cd /tmp/workdir-demo  cd won't switch to directory so is workdir we use
WORKDIR /tmp/workdir-demo
RUN pwd
RUN echo "Hello I am in work dir" > hello.txt
CMD ["sleep","1000"]