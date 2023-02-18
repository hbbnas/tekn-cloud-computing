## Bridge Networking


### Step 1: The Basics
<img src="../images/Listing_Network.jpg" alt="Git Version" style="max-width: 100%;">


### Step 2: Connect a container

``Create a new container by running docker run -dt ubuntu sleep infinity.``


<img src="../images/Install-Image-Ubuntu.jpg" alt="Git Version" style="max-width: 100%;">


``You can verify our example container is up by running docker ps.``


<img src="../images/Ubuntu-Network.jpg" alt="Git Version" style="max-width: 100%;">


### Step 3: Test network connectivity

``Lets run a shell inside that ubuntu container, by running docker exec -it <CONTAINER ID> /bin/bash.``


<img src="../images/Exec-Container.jpg" alt="Git Version" style="max-width: 100%;">


``Ping github``


<img src="../images/Ping-Github.jpg" alt="Git Version" style="max-width: 100%;">


### Step 4: Configure NAT for external connectivity

``Start a new container based off the official NGINX image by running docker run --name web1 -d -p 8088:80 nginx.``


<img src="../images/Create_New_Container.jpg" alt="Git Version" style="max-width: 100%;">


``You can connect from your Docker host using the curl 127.0.0.1:8088 command.``


<img src="../images/Curl.jpg" alt="Git Version" style="max-width: 100%;">