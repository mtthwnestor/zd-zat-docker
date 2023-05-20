# zd-zat-docker

Zendesk Apps Tools allow you to perform actions locally, such as previewing a Help Center Theme locally.

## Build

Build with the following command: 

```bash
docker build -t zat -f Dockerfile.zat .
```
## Use

Following along with [Zendesk's instructions](https://support.zendesk.com/hc/en-us/articles/4408822095642), use this command to start the preview process:

```bash
docker run --rm -it -v $PWD:/app -p 4567:4567 zat zat theme preview
```
