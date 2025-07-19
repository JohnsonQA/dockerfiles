#ARG is also same as env which we can use to pass varibale values
#But env varibales can be used inside container and also build time varibale where ARG varibale are build time varaibles
#In an exceptional case arg can be first instruction to suplly version to the base OS in FROM, we can't use this
# after from instrction

#If we wann use ARG inside a container then we can pass the ref varibale of ARG to ENV instruction
#If we don't give any version in ARG then default version in FROM it will take
#AR$G variables can be overriden
ARG version
FROM almalinux:${version:-9}
ENV course="devops" \
    duration="120hrs"
ARG trainer="sivakumar"
ENV trainer=$trainer
RUN echo "Hi, Course is: ${course}, duration is: ${duration}, trainer is: ${trainer}, version: ${version}"
CMD ["sleep", "1000"]