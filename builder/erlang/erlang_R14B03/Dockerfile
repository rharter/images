FROM bradrydzewski/kerl

WORKDIR /home/ubuntu
USER ubuntu
ADD kerl.sh /etc/drone.d/

RUN kerl build R14B03 R14B03 && \
	sudo mkdir /opt/R14B03 && \
	sudo chown -R 1000:1000 /opt/R14B03 && \
	kerl install R14B03 /opt/R14B03