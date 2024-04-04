## TBC
```
sudo apt install docker-buildx-plugin
```
```
docker buildx create --use --platform=linux/arm64,linux/amd64 --name multi-platform-builder
docker buildx inspect --bootstrap
```
```
docker buildx build --platform linux/amd64,linux/arm64  -t dockersec/siege --push .
```
