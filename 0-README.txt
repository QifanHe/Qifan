ENG ECE EC 601 Homework 1
  Team members:
    Qifan He (heqf@bu.edu , @qifanhe on Slack)
    Robert Munafo (rmunafo@bu.edu , @mrob27 on Slac

Project links:
  Trello:   https://trello.com/b/axu9ZZZZ/hw1-1st-sprint
  Github:   https://github.com/QifanHe/Qifan
  Slack:
    @qifanhe (Qifan He)
    @mrob27  (Robert Munafo)

----

Source files are from OpenCV version 3.1.0. Get a copy of the source code:

  git clone https://github.com/Itseez/opencv.git

Full instructions for installing OpenCV on a Linux system (Ubuntu 16.04)
were found at:

  www.pyimagesearch.com/2015/06/22/install-opencv-3-0-and-python-2-7-on-ubuntu/

We also found instructions for installing on Windows, and Mac install
instructions were posted on Blackboard.

Once you have followed the OpenCV instructions, you can create a
folder for this project by "cloning" the Github repository, or by
downloading a ZIP archive from the Github website and un-ZIPing it on
your machine.

In Linux, the install instructions involve setting up virtualenv; to
run a Python program that uses OpenCV one has to first type "workon
cv" to enter the virtualenv that has the OpenCV packages. Then "python facedetect.py"
wiull start the demo. It opens a window showing the webcam's image, with faces
and eyes highlighted by green rectangles.

The files we used came from these paths within the OpenCV source tree:

  opencv/samples/python  (the three .py files)
  opencv/data/haarcascades  (the two .xml files)

----
 20160914.1750

Qifan already added me as a collaborator (we did that yesterday) on github. Today I added
the first file, 0-README.txt. Here is the console log:

 - - - start - - -

(cv) munafo@morobu:~/EC601/HW1/facedetect$ python facedetect.py 

face detection using haar cascades

USAGE:
    facedetect.py [--cascade <cascade_fn>] [--nested-cascade <cascade_fn>] [<video_source>]

^CTraceback (most recent call last):
  File "facedetect.py", line 59, in <module>
    rects = detect(gray, cascade)
  File "facedetect.py", line 25, in detect
    flags=cv2.CASCADE_SCALE_IMAGE)
KeyboardInterrupt
(cv) munafo@morobu:~/EC601/HW1/facedetect$ emacs 0-README.txt
(cv) munafo@morobu:~/EC601/HW1/facedetect$ git init
Initialised empty Git repository in /media/munafo/S32/bmd/EC601/HW1/facedetect/.git/
(cv) munafo@morobu:~/EC601/HW1/facedetect$ git add 0-README.txt 
(cv) munafo@morobu:~/EC601/HW1/facedetect$ git commit -m "new project for HW1, add README file"

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'munafo@morobu.(none)')
(cv) munafo@morobu:~/EC601/HW1/facedetect$ git config --global user.email "mrob27@gmail.com"
(cv) munafo@morobu:~/EC601/HW1/facedetect$ git config --global user.name "Robert Munafo"
(cv) munafo@morobu:~/EC601/HW1/facedetect$ git commit -m "new project for HW1, add README file"
[master (root-commit) 0d578d0] new project for HW1, add README file
 1 file changed, 12 insertions(+)
 create mode 100644 0-README.txt
(cv) munafo@morobu:~/EC601/HW1/facedetect$ git remote add origin https://github.com/QifanHe/Qifan.git
(cv) munafo@morobu:~/EC601/HW1/facedetect$ git push -u origin master
Username for 'https://github.com': mrob27
Password for 'https://mrob27@github.com': 
Counting objects: 3, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 413 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/QifanHe/Qifan.git
 * [new branch]      master -> master
Branch master set up to track remote branch master from origin.
(cv) munafo@morobu:~/EC601/HW1/facedetect$ 

 - - - end - - -

----
 20160916.1805

To make a copy of the same files on another machine I had to do this:

  SB4 /Users/munafo/EC601/HW1/facedetect 
   : git clone https://github.com/QifanHe/Qifan.git
  Cloning into 'Qifan'...
  remote: Counting objects: 13, done.
  remote: Compressing objects: 100% (10/10), done.
  remote: Total 13 (delta 3), reused 12 (delta 2), pack-reused 0
  Unpacking objects: 100% (13/13), done.
  SB4 /Users/munafo/EC601/HW1/facedetect 
   : mv Qifan facedetect

then I added this text to 0-README.txt. To update the central repository
I will do this:

  git add 0-README.txt
  git commit
  # It puts me in an editor, I type a message explaining that I
  # added this text, then save, then quit the editor
  git push
  # enter my github user ID and password

----

