# Formation Docker and Ansible

## Setup

- Install [docker](https://docker.com) and [docker-compose](https://docs.docker.com/compose/)

```bash
# Download Docker
$ curl -fsSL https://get.docker.com -o get-docker.sh
$ sh get-docker.sh

# Install docker-compose
$ sudo curl -L "https://github.com/docker/compose/releases/download/1.25.5/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
$ sudo chmod +x /usr/local/bin/docker-compose

$ sudo usermod -aG docker $USER
```

## Docker

## Ansible

### [Workshops](./ansible/workshops/README.md)
