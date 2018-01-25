docker-hello-world
==================

An updated image from the tutumcloud/docker-hello-world repo. This is a very basic Hello World image that we use to test the Automated build of the Dockerfile and the auto deployment of the updated container via Tutum.

Check out the full article on how to automate docker builds end-to-end: [Brianchristner.io](https://www.brianchristner.io/how-to-automate-docker-builds-end-to-end/)


Usage
-----

To create the image `vegasbrianc/docker-hello-world`, execute the following command on the docker-hello-world folder:

	docker build -t vegasbrianc/docker-hello-world .

You can now push your new image to the registry:

	sudo docker push vegasbrianc/docker-hello-world


Running your Hello World docker image
-------------------------------------

Start your image:

	sudo docker run -d -p 80 vegasbrianc/docker-hello-world

It will print the new container ID (like `d35bf1374e88`). Get the allocated external port:

	sudo docker port d35bf1374e88 80



