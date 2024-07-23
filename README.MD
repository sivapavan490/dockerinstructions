
FROM :-

* FROM is the 1st instruction of the docker file always. Because  by using FROM instruction only we are taking the base image.

RUN :-

* RUN instruction is used at the image building time ,while doing the software instructions are configurations on the image

CMD :-

* CMD instruction is used to make our container running .
* If container is running then only we can acess the container by outside world. 



LABEL :-

* Label instruction adds meta data to an image.simply we are using mostly labels for filter the images

EXPOSE:-

* EXPOSE instruction informs docker that the container listens on the specified n/w ports at run time
This instruction is used for just information purpose only. IT DOES NOT OPEN ANY PORT

ENV :-

* env is the environmental variables of  the container. if we mention the env variables in docker file. That env variables are belong to that image or container.

COPY :-
* copy instruction is used to copy files from local to the image.

ADD:-

* 

COPY VS ADD :- (preference is ADD)

* Both COPY & ADD instructions are used to copy the files from local to image
* But ADD instruction has extra 2 capabilities. They are :-
    1) It can directly downnload the files from internet.
    2) It can directly untar the tar files.

RUN VS CMD :-
* run instruction runs at  the time of image building.
* cmd instruction runs at the time of container creation.

CMD VS ENTRYPOINT :-
* Both CMD & ENTRYPOINT instructions are work at container  creation time only.
* But CMD Instruction can be over-ridden by another command at run time.
* ENTRYPOINT Instruction can't be overridden at any point,if u try to do the cmd u r entering at eun time will go and append to entrypoint.

WORKDIR :- 

* This instruction is used to change the directory of container.

ARG :-

* ARG instruction can be used before FROM instruction to provide values to FROM instruction.
