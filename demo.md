===================================
WEDNESDAY SUBSYSTEM FOR LUNCH (WSL)
===================================

Things to mention at the top:
-----------------------------
- This study hall will give a very brief conceptual introduction to WSL,
  before moving into the practical pieces you should know for your time
  at Rithm.
- We will have a window (no pun intended) of time at the end for you to ask
  questions and share any issues you've run into that we did not touch on.


Show of hands:
--------------
- Who has used Linux?
- Who knows what a virtual machine is?


Terminology
-----------
***Linux***: a family of Unix-like operating systems.
***Ubuntu***: a popular and beginner-friendly distribution ("distro") of Linux.
(This is the the distro we have you install.)
***WSL***: architecture that allows Linux to run natively under Windows.
***Virtual machine***: emulated version of an operating system.

You can think of WSL as a super lightweight virtual machine
that allows you to run Ubuntu Linux in its own box, *within* Windows.


Filesystems
------------
Your Linux files are not kept in your normal Windows home folder;
instead, WSL sets up a separate filesystem for them.

<pre>
        [/]
[Windows]  [Linux]
    /         \
   /           \
  /             \
 mnt           home
  |              |
  c          ~ stocktons
  |              |
Users          rithm
  |              |
stock        assessments
  |
Downloads
</pre>

You will run into performance issues if you try to work on files within the
Windows filesystem from your Linux shell, and vice versa.

For this class, since you are working within WSL, you will want to make sure
your files are created within or moved to that filesystem as soon as possible!


Moving Things Into Ubuntu
-------------------------
You can move downloaded files from your Windows *Downloads* folder over to your
Linux filesystem in one of two ways:
- TODO: DISCUSS WAY 1 (GUI; don't show them this?)
- TODO: DEMO WAY 2 (suggested, within your shell)

You can move them back, should you need to, like this:
- TODO: DEMO MOVING BACK (within shell)


Zipping/Unzipping
-----------------
Don't unzip on the Windows side! You'll end up with a million "ZoneIdenifier"s.
These files aren't dangerous, but they are annoying.

Most of our exercises and assessments are a single zip file. Once you've moved
this zip file into your Linux filesystem, you can extract the contents with:
` ~ unzip <dir_name_here.zip>`

You can zip a directory with:
` ~ zip <dir_name_here>`

As part of the pre-work, we also set you up with the shell command `zipsubmit`!
This will zip your assessment work, automatically ignoring common undesireable
files and folders that you'd otherwise have to manually omit.


Deleting things
---------------
Same old command:
`~ rm -rf <dir_name_here>`


LiveServer
----------
LiveServer is a convenient tool that allows you to fire up a bare-bones server
within VS Code.

We currently do not ensure that LiveServer functions out of the box
with our WSL setup.

That's intentional; we want you to use other server tools that we will show you,
like Python's *http.server* module.


VS Code Terminal
----------------
Depending on your exact setup, your VS Code terminal might start in Powershell.

Regardless of whether it initially appears as Powershell or your Linux shell,
we will encourage EVERYONE to use the standalone shell.

Get in that habit now instead of worrying about the VS Code terminal!


In summary:
-----------
This is the way we've had you set up WSL so you can work with our
curriculum effectively; there's way more here, but it's not necessary for now.


Questions?
----------


> TODO:
@Sarah: put things into Rithm slides w/ visuals
@Edmond: Double check that http.server hot reloads.
@Both: test moving files for demo