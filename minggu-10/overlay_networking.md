## Overlay Networking


### Step 1: The Basics

``Run a docker node ls to verify that both nodes are part of the Swarm.``

<img src="../images/Swarm.jpg" alt="Git Version" style="max-width: 100%;">

### Step 2: Create an overlay network

``Create a new overlay network called “overnet” by running docker network create -d overlay overnet.``


<img src="../images/new_network.jpg" alt="Git Version" style="max-width: 100%;">


### Step 3: Create a service

``Now that we have a Swarm initialized and an overlay network, it’s time to create a service that uses the network.``

<img src="../images/services.jpg" alt="Git Version" style="max-width: 100%;">


### Step 4: Test the network

<img src="../images/exec.jpg" alt="Git Version" style="max-width: 100%;">
<img src="../images/ping.jpg" alt="Git Version" style="max-width: 100%;">
