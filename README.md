# Install (OSX)

##### Install plugin (sublime text 3)

Navigate to the packages directory default:

    cd /Users/{user}/Library/Application Support/Sublime Text 3/Packages

Clone the repo:

    git clone https://github.com/mbarkhau/SublimeQueryDB.git

##### Install postgres:

    brew update
    brew install postgres

##### Setup a pgpass file

Set up a pgpass file in your home directory.  Entries are of the form:

    hostname:port:db:user:password

Make sure to set the permissions to 600 (or less)

    chmod 600 ~/.pgpass

##### Other Notes

Check the sublime text console output (View -> Show Console), you may have to edit query_db to point to your psql from root:

    "psql" --> "/usr/local/bin/psql"