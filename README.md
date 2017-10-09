# Freeflow Starter Kit

> A starting repository leveraging [Docksal](https://github.com/docksal) for a local dev environment.

## Requirements

* [Composer](https://getcomposer.org/download) (e.g. `brew install composer`)
* [Docksal](http://docksal.io)

## Installation
### Local virtual machine
Download docksal.

    $ curl -fsSL get.docksal.io | sh
Download and install docksal virtualbox VM. (this may take a while)

    $ fin vm start

### Repository setup
Clone the Freeflow StarterKit repository.

    $ git clone  git@github.com:FreeflowDigital/Drupal8-advanced [project name]
    $ cd [project name]

Install Drupal site with Docksal.

    $ fin init

### Drupal Console
Initialize and test that the console is working:

    $ fin console init
    $ fin console cr

`cr` is an alias for cache rebuild (cache clear in d7), i.e. `fin console cache:rebuild`.

#### Usage
Existing sites run:

    $ fin console config:import
    $ fin console update:entities

See handy cheat-sheet for Drupal Console commands [here](https://drupalconsole.com/cheatsheet/).
