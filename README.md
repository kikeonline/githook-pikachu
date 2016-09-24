# githook-pikachu
[githooks](https://git-scm.com/docs/githooks) - post-receive: Script that gets excecuted when the server receives a push. Can be use to automate tasks that have to be made after a push is done.
<img src="https://github.com/kikeonline/pikachu-githook/blob/master/terminal-screen.png" width="600">

# Instalation
Copy the post-receive script to .git/hooks probably you already have some example files there.

Give excecutable permissions.
  ```bash
  $sudo chmod +x post-receive
  ```

I used this file as a base to make more complex tasks. In this particular script if the push comes from a master branch I copy all the master files from the bare repo to /www/html where my web files are served. Else (another branch) files are simply saved and no deploy is done. Most importantly Pikachu greets the pusher.

Used it to fulfill your needs, You can even send push notifications to your smartphone through [Pushover](https://pushover.net). imagination is the limit ✌️
