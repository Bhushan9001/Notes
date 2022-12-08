
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
```
pwd
```
```bash
docker push docker-registry-username/docker-image-name
```
Install and configure Jenkins to build job integrating with github
```bash
Go to your Jenkins profile
Click on New item
Give name and select freestyle project then Done
Go to source code management
Then click on git
Enter repository url
Then in build triggers
Check the GitHub hook trigger.......
Then click on save
After that in build history
Check console output
```
