# Purpose

insert-time provides an easy way to insert time and date stamps into
your files

## Usage

Example of lines to be added to your .emacs:

    (require 'insert-time)

    ; in case you don't like the defaults
    ; (see `format-time-string' for format)
    (setq insert-date-format "%Y-%m-%d")
    (setq insert-time-format "%H:%M:%S")

    ; keyboard shortcuts
    (define-key global-map [(control c)(d)] 'insert-date-time)
    (define-key global-map [(control c)(control v)(d)] 'insert-personal-time-stamp)

## How it works

just a few inserts using the emacs built in format-time-string
