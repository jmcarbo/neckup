neckup - For autist neckbeards (TM)
===================================

Simple upload service using cURL or form.

GOALS:
  * No framework,
  * No JS,
  * No database,
  * Follow KISS-principles,
  * Try to be neckbeardish?

CONTRIBUTE:
  The project is open for contributions and neckbeardnes. Feel free to
  contribute as long as you follow the goals (somewhat atleast).

  I'm kind of new to the Go language so you shouldn't be surprised to find
  weird practices that do not fit the language, please create an issue or a
  pull request if there's something to improve.

BUILD:
  go build

TEST:
  go test

RUN:
  ./neckup

HELP:
  ./neckup --help

SETUP:
  This setup uses a neckup user where everything is placed
  in its home directory (/home/neckup/neckup/).

  You should already have setup a Nginx web server.

    * Create and setup the neckup user,
        - $ useradd -m neckup
        - $ su neckup
        - $ cd ~

    * Get the latest version of neckup and cd into it,
        - $ git clone git@github.com:willeponken/neckup.git
        - $ cd neckup

    * Compile neckup.go and show the different flags available,
        - $ go build neckup.go
        - $ ./neckup --help

    * Create seperated or merged nginx server block(s),
        - see examples/nginx/neckup_*
    
    * Optionally add an init script for the process.
      Feel free to add more scripts in "examples/",
        - see examples/upstart/neckup_*.conf (upstart)

    * Reload Nginx and start neckup and you should be good to go!

DEMO:
  * Internet: https://nup.pw/
  * Hyperboria: http://h.nup.pw/
    - No ICANN: http://[fcf5:894b:a246:fa31:f395:6e8d:31b6:f9f9]/ (note: the
      web server still uses the ICANN domain)

TODO:
  See /TODO.txt

LICENSE:
  GPL-3.0 (can be found at /LICENSE)
