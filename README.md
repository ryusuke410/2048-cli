#2048-cli

A cli version/engine of the game [2048](https://github.com/gabrielecirulli/2048) for your Linux
terminal.

![Screenshot](http://i.imgur.com/QU7t5mH.png)

There currently are 3 versions that can be run. These include a straight-forward terminal
based, and two using the ncurses and SDL libraries. To add a new graphical version, simply
create a .c file which implements all the functions in gfx.h and add a Makefile entry.

### Get
    git clone https://github.com/Tiehuis/2048-cli.git
    make

You can easily install this on el >= 5 (CentOS, RedHat Enterprise Linux,
Scientific Linux, Oracle) and Fedora >= 19 using the package-manager:

    sudo yum install 2048-cli[-nocurses]

For el you will need to have the
[EPEL-repository](https://fedoraproject.org/wiki/EPEL/FAQ#How_can_I_install_the_packages_from_the_EPEL_software_repository.3F)
enabled.

### Run
    ./2048

## Options
    -s <size>      Set the grid border length
    -b <rate>      Set the block spawn rate
    -r             Resets hiscore. Will prompt user
    -c             Enables color support (ncurses version only)
    -C             Disables color support (ncurses version only)

Fonts used in SDL version can be found [here](http://www.openfontlibrary.org).

## License
This code is licensed under the
[MIT License](https://github.com/Tiehuis/2048-cli/blob/master/LICENSE).
