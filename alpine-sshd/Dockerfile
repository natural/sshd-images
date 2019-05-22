FROM alpine:latest

RUN apk update && apk add openssh
RUN ssh-keygen -A
RUN mkdir -p ~root/.ssh 
RUN echo -e "root\nroot" | passwd root
RUN sed -i 's/#PermitRootLogin prohibit-password/PermitRootLogin without-password/' /etc/ssh/sshd_config

EXPOSE 22
CMD ["/usr/sbin/sshd", "-D"]
