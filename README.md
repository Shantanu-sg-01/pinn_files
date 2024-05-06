# phygeonet env
https://drive.google.com/file/d/1zD00jkQEwWpa6isfzdNCSwu0B454nI5Q/view?usp=sharing

# foam pinn os
https://drive.google.com/file/d/1Ld7-bjrxbIbJG7tsE-_NEw3_BT4BLn9s/view?usp=sharing

# additional installation files
https://drive.google.com/drive/folders/1-yvHW5T194rbXaxZwWPmms27WOra0nYN?usp=sharing

# libtorch tutorials
https://drive.google.com/file/d/16921MqAS89t-knz-uX02H9PMbPOhmlv6/view?usp=sharing


instructions for loading image
You will need to save the Docker image as a tar file:

docker save -o <path for generated tar file> <image name>
Then copy your image to a new system with regular file transfer tools such as cp, scp, or rsync (preferred for big files). After that you will have to load the image into Docker:

docker load -i <path to image tar file>
You should add filename (not just directory) with -o, for example:

docker save -o c:/myfile.tar centos:16
your image syntax may need the repository prefix (:latest tag is default)

docker save -o C:\path\to\file.tar repository/imagename
PS: You may need to sudo all commands.
