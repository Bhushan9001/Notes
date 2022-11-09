
## Docker Installation



```bash
  sudo apt-get update 
```
```bash
  sudo apt install apt-transport-https ca-certificates curl software-propertiescommon
```
```bash
sudo mkdir -p /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
```
```bash
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-compose-plugin
```
```bash
sudo docker run hello-world
```
```bash
docker images
```
```bash
docker ps -a
```
```bash
docker rename <container-name> <any-name>
```
```bash
docker commit -m "What you did to the image" -a "Author Name" container_id
repository/new_image_name

```
```bash
docker login -u docker-registry-username
```
```bash
docker push docker-registry-username/docker-image-name
```
