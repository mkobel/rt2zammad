# rt2zammad

Request tracker to Zammad migration script. This is not an out of box solution
for everybody, you will probably have to customize it.

Known issues:

* Disabled users from RT can not be accessed by API, thus will lack email
  address and will fail to be created. Enable all users prior to the migration.
* Timestamps are not preserved. The Zammad API doesn't seem to allow this.
* Zammad will send notification for all actions, you probably want to disable
  outgoing mail for time of import.
