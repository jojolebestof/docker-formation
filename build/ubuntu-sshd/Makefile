
DOCKER_IMAGE=albttx/ubuntu-sshd
TAG=18.04

.PHONY: all build deploy

all: build deploy

build:
	docker build -t $(DOCKER_IMAGE):$(TAG) .

deploy:
	docker push $(DOCKER_IMAGE):$(TAG)

