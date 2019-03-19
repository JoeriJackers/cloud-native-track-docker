FROM centos:7.6.1810

LABEL maintainer="joeri.jackers@kbc.be"
LABEL licence="GPL"

RUN for i in {0..30}; do echo "$i"; sleep 1; done; echo

ARG hello_world_string

RUN touch /hello-world.txt &&\
	echo "{hello_world_string}" > /hello-world.txt

CMD ["cat", "/hello-world.txt"]
