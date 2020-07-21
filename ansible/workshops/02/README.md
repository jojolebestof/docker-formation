# WORKSHOP 02

## Setup

### Start a simple ubuntu

```bash
# Add ssh-key into your agent
$ ssh-add ../../../build/ubuntu-sshd/ubuntu-sshd
Identity added: ../../../build/ubuntu-sshd/ubuntu-sshd (albttx@think-p1)

$ docker-compose up -d
```

### Check the server is up and running

```bash
# test you have ssh access to the servers
$ ssh root@172.21.1.4
root@467a3d1e055b:~#
^C

# test ansible ping
$ ansible -m ping all
ansible01 | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python3"
    },
    "changed": false,
    "ping": "pong"
}
```

## Exercices

1. Create a role that will install and run a traefik proxy inside the container

```bash
$ curl http://172.21.1.4:8080
Moved Permanently

# Open your browser on http://172.21.1.4:8080 to see the dashboard
```
