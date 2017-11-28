Atramhasis demo docker
======================

A dockerfile to build an Atramhasis demo docker image.

Run a Atramhasis demo instance
------------------------------

After installing Docker for your operating system, you 
can simply pull the image and run a container. After
executing the following commands you should be able to 
visit the demo application in your browser on 
http://localhost:6543. A LDF-server is also included
in the demo and accesible on http://localhost:3000.

.. code::

   $ sudo docker pull atramhasis/demo
   $ sudo docker run -p 6543:6543 -p 3000:3000 atramhasis/demo



Build and run an image
----------------------

This is *not necaserry* if you just want to run the demo in a 
container. You can pull the image from https://hub.docker.com.

.. code::

  $ sudo docker build -t atramhasis/demo .
  $ sudo docker run -p 6543:6543 -p 3000:3000 atramhasis/demo
