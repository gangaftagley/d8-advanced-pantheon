# Database Operations

The `db_key` argument is optional in these commands. The default defined in `settings[.local].php` will be used if no key is specified.

**Dump:**

Note that the `db` directory must exist at the same level as `docroot`.

    $ fin console database:dump --file=../db/dump.sql [db_key]
    
**Drop:**
    
    $ fin console database:drop [db_key]
    
**Import/Restore:**

~~fin console database:restore --file=../db/dump.sql [db_key]~~

`database:restore` doesn't work as expected. For now, move the dump into the docroot and use drush directly in the VM:

    $ cp db/dump.sql docroot/
    $ fin bash
    $ cd docroot
    $ drush sql-cli < dump.sql
