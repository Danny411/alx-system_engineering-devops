#!/bin/bash
This whole new file will contain all shell permissions commands and how they are been used respectively

su betty  .....  a script that switches the current user to the user betty [assuming betty to be the user name to be switched to.

whoami   ..... a script that prints the effective username of the current user.

groups  ...... a script that prints all the groups the current user is part of.

sudo chown betty hello  ..... a script that changes the owner of the file hello to the user betty

touch hello   ...... a script that creates an empty file called hello.

chmod u+x hello  .... a script that adds execute permission to the owner of the file hello.

chmod +114 hello ..... a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.

chmod +111 hello ..... a script that adds execution permission to the owner, the group owner and the other users, to the file hello

chmod 007 hello ..... a script that sets the permission to the file hello as follows: [Owner: no permission at all , Group: no permission at all, Other users: all the permissions]

chmod 753 hello .... a script that sets the mode of the file hello to this [-rwx-x-wx]


chmod --reference olleh hello ..... a script that sets the mode of the file hello the same as olleh’s mode. [ hello mode " -rwx-x-wx" , olleh mode "-rw-rw-r--" ]

chmod a+x / ..... a script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed.


mkdir -m 751 my-dir  ....  a script that creates a directory called my_dir with permissions 751 in the working directory.


chgrp school hello  .... a script that changes the group owner to school for the file hello


chown vincent:staff *  .....  a script that changes the owner to vincent and the group owner to staff for all the files and directories in the working directory.

chown -h vincent:staff _hello .....  a script that changes the owner and the group owner of _hello to vincent and staff respectively.


chown  --from=guillaume betty hello .... a script that changes the owner of the file hello to betty only if it is owned by the user guillaume.


telnet towel.blikenlights.nl .... a script that will play the StarWars IV episode in the terminal.
