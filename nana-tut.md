# YAML Tutorial

## What is YAML?
YAML Ain't MarkUp Language, is a data serialization language. Other examples are json, xml, etc. YAML is the cleanest & most human readable of them all.
## YAML Use Cases
Docker, Kubernetes, Ansible, Prometheus, etc. configuration files all written in YAML.

## Basic Syntax of YAML

### Key-Value Pairs
```yaml
# this is a comment
app: user-authentication
port: 9000
version: 1.7
```

### Objects
```yaml
# Objects are indented items
microservice:
  app: user-authentication
  port: 9000
  version: 1.7

# Creating Lists of Objects or microservices for example
microservices:
  - app: user-auth
    port: 80
    deployed: false
    requirements:
      username: sakib
      password: 12345

  - app: user-login
    port: 90
    deployed: true
    requirements:
      token:
        timeout: 10
        signed: false
        validate: [sakib, prangon, sahadat, mehedi]


```

* [YAML Techniques Video Tut](https://www.youtube.com/watch?v=1uFVr15xDGg)
