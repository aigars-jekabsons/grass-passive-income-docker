# Grass Passive earning Docker solution.
This solution uses chromium base image.  with pre installed VNC.
It has been fully tested on x64 system and on Rasperry PI 4B. Unfortunately on ARM CPU chips container crashed every other day.

Here is their website for more information https://www.getgrass.io/

# Pre requisites 
Docker has to be pre installed on the system.

# Step by step guide in using this docker-compose file

###### 1. Clone the repo with docker-compose.yaml
#
#
###### 2. change docker-compose.yaml line 21 to source location for cache files. This can be any location on your system. If this step is missed then after rebooting your system you will have to download grass extension again will have to login again.
#
if on windows the line 21 should look something like this : source: C:\chromium-grass
if on linux the line 21 should look like something like this : source: /chromium-grass


###### 3. Run docker-compose up from the same folder where docker-compose.yaml is located 
you can do so by running command:
```sh
docker-compose up -d
```
-d stands for detached so the docker image would run in background.

###### 4. Once Docker image is up and running open your browser and navigate to http://localhost:3000/

This will navigate you into the container chrome browser. And grass extension page should already be openned.

###### 5. Install grass extension on docker chrome browser by clicking Add to chrome. This will ask you to add Grass extension to the browser. just confirm it

###### 6. Once extension has been installed just click on the extension in the chrome toolbar. It will ask you to sign in.
###### 7. Next step is to create getgrass account. Because this platform has been recently launched it is still just an open beta. You can register only by an invite. Here is a link where you will be able to create an account: [Grass Registration Page with Invite](https://app.getgrass.io/register/?referralCode=uUbOBprERCXVr5n)
###### 8. After registration navigate back to Docker Container and Login inside of the extension and that is it. Enjoy Grass Passive Income in docker.

if you like what you see drop me an email with a thumbsup to aigarsaj@gmail.com