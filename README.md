
# Cboard-Boostrapp  

[Cboard](https://app.cboard.io/) is an augmentative and alternative communication (AAC) web application, allowing users with speech and language impairments (autism, cerebral palsy) to communicate by symbols and text-to-speech. This repo supports the CBoard front-end, providing backend functionality and persistence.

Docker bootstrap provides an easy way to manage the cboard container.


## How to use it

To build the boostrap image:

```
docker build -t cboard-bootstrap .
```

To start up the container:
```
docker run --rm -v /var/run/docker.sock:/var/run/docker.sock cboard-bootstrap up -d
```

To stop the container:
```
docker run --rm -v /var/run/docker.sock:/var/run/docker.sock cboard-bootstrap down
```