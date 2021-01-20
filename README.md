# soundcloud-likes
Download all the songs from your SoundCloud Likes

![Image of Downloads](http://imgur.com/L7yTzzH.png)

Running this script will download all of the songs in your soundcloud likes in a directory named `songs`.

A file named `downloaded.txt` will be created which keeps tracks of all the files you have successfully downloaded

A file named `errors.txt` will be created which keeps tracks of all the songs that errored out on download

Optionally, you can create a file within the `soundcloud-likes-master` directory called `ignored.txt` that has soundcloud links that should be ignored.

## Setup (Mac)

The instructions I'm giving assume that you are non-technical. If you know about directory structures and how to use Terminal,
customize install for your own preferences

1.) Click the green 'Clone or download' button at `https://github.com/drivelous/soundcloud-likes` and download the ZIP onto your Desktop

2.) Extract the deepest `soundcloud-likes-master` folder onto your desktop.

3.) Open up Terminal. Press command + spacebar to open up Spotlight Search and type 'terminal'. Open up the first application (Terminal) that pops up

4.) In the prompt type `cd ~/Desktop/soundcloud-likes-master` (or whatever the folder is named).

5.) In the prompt type `pip install virtualenv`. You might already have it but do it just in case.

6.) In the prompt type `virtualenv venv2`. This should create a virtualenv directory named `venv2`.

7.) In the prompt type `source venv2/bin/activate`. This will activate the virtualenv so that the packages you are about to install are not downloaded globally

8.) In the prompt type `pip install -r requirements.txt`

9.) Once that's successful, you can run the script by typing `python main.py <soundcloud_user_name_here>`. Find your username by going to your profile and looking at the URL

## Setup (Windows)

1.) Click the green 'Clone or download' button at `https://github.com/drivelous/soundcloud-likes` and download the ZIP onto your Desktop

2.) Extract the deepest `soundcloud-likes-master` folder onto your desktop.

3.) Download and install git for windows at: `https://gitforwindows.org/`

4.) Then, in the Cortana search field (Win + S), type in Command Prompt, or just CMD.
    Right click the top result, and select Run as Administrator.

5.) Type `pip install virtualenv`

4.) Open the `soundcloud-likes-master` folder, then right click and select 'Git Bash Here'

5.) Go to your Git Bash window and type `virtualenv venv2`. This should create a virtualenv directory named `venv2`.

6.) In the same git bash window type `source venv2/Scripts/activate`. This will activate the virtualenv so that the packages you are about to install are not downloaded globally

7.) In the same git bash window `pip install -r requirements.txt --user`

8.) Once that's successful, you can run the script by typing `python main.py <soundcloud_user_name_here>`. Find your username by going to your profile and looking at the URL
