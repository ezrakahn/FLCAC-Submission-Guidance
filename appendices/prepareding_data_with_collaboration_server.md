Fetch & Commit Workflow

For team members to coordinate maintenance and curation of FLCAC
repositories, the openLCA desktop application allows changes to be made
to, viewed, and/or retrieved from the remote server. The desktop
application uses the term “Commit” to refer to the action of committing
local changes to the server; whereas, the term “Fetch” is for retrieving
server versions to the local desktop. Any changes and curation comments
may also be viewed remotely and/or synced to or from the local server.
Server comments may be reviewed without affecting a local database but
to reflect in a local database those commits made by other team members
to server repositories, users must “fetch” changes and use the “Diff
Tool.” The Diff Tool displays the differences between the local version
of a database and that of the associated server repository.

To fetch changes from a server repository, right-click on the desktop
database in openLCA and select ***“Repository \> Fetch.”*** If no
changes have been committed by other team members, you will see a
message “Up to date – No changes fetched.” If updates or changes have
been made by team members, you will see a list of changes to be fetched,
which provides a summary of changed and/or new elements. Once you select
“OK,” the “Diff Tool” window will display. This tool allows you to
review changes and either accept the server changes or retain the local
desktop status of each element. Simply, select “move from right to left”
to accept the changed element from the server and “mark as merged” to
reject the server change and retain the current element of the local
version. FLCAC recommends fetching changes with a frequency appropriate
for the activity frequency of the team to maintain transparency and
clarity of tracing changes and avoiding conflicts.