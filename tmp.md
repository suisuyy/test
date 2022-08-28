https://gist.github.com/suisuyy/d69d11f06fd644f46580a76af1e7790a

sudo docker run --rm  -it --shm-size=512m -p 6901:6901 -e VNC_PW=password kasmweb/desktop:1.11.0-rolling
The container is now accessible via a browser : https://<IP>:6901

    User : kasm_user
    Password: password
