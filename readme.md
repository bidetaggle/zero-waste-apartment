# Memo for bidetaggle

- https://www.stbehrendtyoga.com/
- https://greecetest.squarespace.com/
- https://fr.squarespace.com/modeles/ -> modele "FOSTER"

# TUTORIAL FOR turtlefox2020

Open your Terminal application located in `Applications/Utilities/Terminal` (under mac OS X)

You have to type the commands below in, it's the best way to talk directly to the computer, by the way the command interpreter is called a `shell` 🐢

Then, let's establish the connection and log into the server
```
ssh <username>@<server>
```
Please replace <username> and <server> by the proper values sent in your email.

It gonna ask for a password, type the one in the email. It's normal that you don't see nothing while you type your password, it's a common standard. The original purpose is security, no one reading your screen can see your password's lenght to guess it.
If you see this:
```
Last login: <current date> from <your ip address>
<time> turtlefox2020@<3 ~
```
BAM you're in :)

welcome to Newark, New Jersey, the server is overseas. Therefore, please be patient when you type a command, you can feel some latencies due to the long physical distance.

Now, you're located in your home root directory that I setup for you. The wave symbole ` ~ ` indicate the root directory.
Let's list what's around us with `ls`:
```
00:18 turtlefox2020@<3 ~ ls
www
```
As you can see, there is only one directory called `www`, let's go in with `cd` (which stand for Change Directory) and check the files around with `ls`:
```
00:32 turtlefox2020@<3 ~ cd www
00:32 turtlefox2020@<3 ~/www ls
fonts  index.html  readme.md
```
Your website is here. You can edit it the main page with `nano index.html`.

Now you can remove the `www/` content with the command `remove`.

With `ls` again, you can verify that the www directory is empty accordingly to the previous command
```
00:32 turtlefox2020@<3 ~/www ls
00:32 turtlefox2020@<3 ~/www
```

To terminate the connection and come back to your computer paradigm, simply type `exit`, you should come back to the Mac OS X command prompt.

You will have to use the command `scp` to copy your files from your computer to the server's folder `www`: https://stackoverflow.com/questions/343711/transferring-files-over-ssh?answertab=votes#tab-top
