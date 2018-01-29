# emacs-daily-events

[![Marmalade](https://img.shields.io/badge/marmalade-available-8A2A8B.svg)](https://marmalade-repo.org/packages/emacs-daily-events)  
[![License](https://img.shields.io/badge/LICENSE-GPL%20v3.0-blue.svg)](https://www.gnu.org/licenses/gpl.html)

An Emacs package to notify you on specified daily occurring events

## Installation

### Manual

Save the file *emacs-daily-events.el* to disk and add the directory containing it to `load-path` using a command in your *.emacs* file like:

    (add-to-list 'load-path "~/.emacs.d/")

The above line assumes that you've placed the file into the Emacs directory '.emacs.d'.

Start the package with:

    (require 'emacs-daily-events)

### Marmalade

If you have Marmalade added as a repository to your Emacs, you can just install *emacs-daily-events* with

    M-x package-install emacs-daily-events RET

## Usage

Set the daily events you want to be notified on as shown below:

    (emacs-daily-events-set-events (list '("0900" "Scrum meeting")
                                         '("1200" "Lunch time")
                                         '("1700" "End of day")))

Enable the `emacs-daily-events-global-mode` by

    (emacs-daily-events-global-mode)

or

    M-x emacs-daily-events-global-mode RET

Emacs will visually notify you when one of the events occur by flashing the
screen a few times.
