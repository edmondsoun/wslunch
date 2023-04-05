MOVING FILES
------------

Move a .zip file from your Downloads to your current location in the Linux shell
(the . is shorthand for "where I am right now"):
`~ mv /mnt/c/Users/<username_here>/Downloads/<zip_name_here> .`

Or, move a .zip file from your Downloads to a specific location,
i.e. rithm/exercises:
`~ mv /mnt/c/Users/<username_here>/Downloads/<zip_name_here> ~/rithm/exercises`

To find your Windows username, from the Linux shell:
`~ cd /mnt/c/Users`
`~ ls`

[view the directories listed and find the one with your username,
usually abbreviated to five characters]


UNZIPPING/ZIPPING
-----------------

Unzip:
`~ unzip <zip_name_here>`

Zip a directory (.zip will automatically be added to the end of the zip file name,
you don't need to include it):
`~ zip -r <dir_name> <desired_zip_name>`

Once you are working with assessments that contain /venv or /node_modules
(not until week three), use this handy command to easily omit those:
`~ zipsubmit -r <dir_name> <desired_zip_name>`


DELETING
--------

A single file:
`~ rm <file_name_here>`

A directory:
`~ rm -rf <dir_name_here>`

