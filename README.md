## - On your Ubuntu Desktop, open a terminal window, and enter the command:

~ sudo curl -fsSL https://get.docker.com |bash ~

## - Now lets install Portainer

## - Run the command: 

~ sudo docker volume create portainer_data ~

## - Then run the command: 

~ sudo docker run -d -p 8000:8000 -p 9000:9000 --name=portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce ~
