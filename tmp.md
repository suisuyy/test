https://index.docker.io/v1/
docker kill $(docker ps -q)
docker pull kasmweb/chromium:1.11.0-rolling



https://gist.github.com/suisuyy/d69d11f06fd644f46580a76af1e7790a

sudo docker run --rm  -it --shm-size=512m -p 6901:6901 -e VNC_PW=password kasmweb/desktop:1.11.0-rolling
The container is now accessible via a browser : https://<IP>:6901

    User : kasm_user
    Password: password

sudo docker run --rm  -it --shm-size=512m -p 6901:6901 -e VNC_PW=password kasmweb/ubuntu-focal-desktop:develop




https://kasmweb.com/docs/latest/install/single_server_install.html


docker pull kasmweb/ubuntu-focal-desktop:1.11.0-rolling
cd /tmp
curl -O https://kasm-static-content.s3.amazonaws.com/kasm_release_1.11.0.18142e.tar.gz
tar -xf kasm_release*.tar.gz
sudo bash kasm_release/install.sh -I  #use -I not preseed img for save space