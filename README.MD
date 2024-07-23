
FROM :-

* FROM is the 1st instruction of the docker file always. Because  by using FROM instruction only we are taking the base image.

RUN :-

* RUN instruction is used at the image building time ,while doing the software instructions are configurations on the image

CMD :-

* CMD instruction is used to make our container running .
* If container is running then only we can acess the container by outside world. 

RUN VS CMD
* run instruction runs at  the time of image building.
* cmd instruction runs at the time of container creation.

LABEL :-

* Label instruction adds meta data to an image.simply we are using mostly labels for filter the images

EXPOSE:-

* EXPOSE instruction informs docker that the container listens on the specified n/w ports at run time
This instruction is used for just information purpose only. IT DOES NOT OPEN ANY PORT

ENV :-

* env is the environmental variables of  the container. if we mention the env variables in docker file. That env variables are belong to that image or container.