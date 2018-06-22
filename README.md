# laravel-redis-socket
Send real time notification to the user using laravel, redis and socket.io and using database

First, after clone you have to create one virtual host.

<h3>Install packages</h3>

<code>npm install express ioredis socket.io --save</code>

<code>composer require predis/predis</code>
<h3>Setting up Redis</h3>

As mentioned above Redis should already be installed but you just need to edit your .env file to tell Laravel to use the correct BROADCAST_DRIVER. Add the following line.

    BROADCAST_DRIVER=redis
<h3>Starting the Servers</h3>

> Open two command line tabs and SSH into Homestead

<code>cd</code> into the root directory of your project

In the first tab, run <code>node socket.js</code>
You should see "Listening on Port 3000"

In the second tab run <code>redis-server --port 3001</code>
You should see a lot of output

<h3>Trying it out</h3>

> Open up two browser windows side by side and in the first one hit the URL:

    http://your-project-name.app/fire

> And in the second:

    http://your-project-name.app/test
    
Keep refreshing the first window and you should see the second page's content increment.

<h6>You're all done!</h6>

If you are stuck somewhere then call me:

devat.karetha@viitorcloud.in (+91 9558335853)

