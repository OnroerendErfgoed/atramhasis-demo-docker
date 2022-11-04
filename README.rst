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

Or if you wish to run a specific version (starting 
from atramhasis 0.6.4), you can run:

.. code::

   $ sudo docker pull atramhasis/demo:0.6.4
   $ sudo docker run -p 6543:6543 -p 3000:3000 atramhasis/demo:0.6.4


Build and run an image
----------------------

This is *not necaserry* if you just want to run the demo in a 
container. You can pull the image from https://hub.docker.com.

.. code::

  $ sudo docker build -t atramhasis/demo .
  $ sudo docker run -p 6543:6543 -p 3000:3000 atramhasis/demo


 Run Atramhasis with docker-compose
-----------------------------------

You can create and start Atramhasis with a single command:

.. code::

  $ docker compose up
