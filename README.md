# Jellyfin docker-compose example
## 1. Install docker
Install docker by following [https://docs.docker.com/desktop/#download-and-install](https://docs.docker.com/desktop/#download-and-install)

## 2. Commands

### Run without logs
```sh
cd jellyfin
docker-compose up -d
```

### Run with logs
```sh
cd jellyfin
docker-compose up
```

## 3. Media files
After setting up, you can place music/movie in the media folder
```sh
./vol/media
```

## 4. Some helpful notes
On Centos7, I had to run following commands after installing docker:
```sh
sudo usermod -aG docker $(whoami)
sudo systemctl enable docker.service
sudo systemctl start docker.service
sudo chmod 666 /var/run/docker.sock
```
