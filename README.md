# Node Development
Creates docker containers based on the official Docker version of [Node.js](https://registry.hub.docker.com/_/node). On top of those images it installs `nodemon` adds an entrypoint of `nodemon` and passes a default argument of `.`.

Supported tags and respective `Dockerfile` links

- `0.10.38-onbuild` `latest` [(0.10.38/onbuild/Dockerfile)](https://github.com/School-Improvement-Network/docker-node-development/blob/master/0.10.38/onbuild/Dockerfile)
- `0.12.4-onbuild` `latest` [(0.12.4/onbuild/Dockerfile)](https://github.com/School-Improvement-Network/docker-node-development/blob/master/0.12.4/onbuild/Dockerfile)

## Usage

```bash
# Run the index.js file in the current folder
docker run -it \
	-v "$PWD":/usr/src/app \
	sinet/node-development

# Run test.js in the current folder
docker run -it \
	-v "$PWD":/usr/src/app \
	sinet/node-development \
	test.js
```
