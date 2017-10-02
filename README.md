# Notes
helper scripts

* As the functionality grows, the number of scripts grow. When time permits, I'll refractor these scripts into usable functions.


./getStatus <processGroupUUID>
Will return the processGroups, and processors.

## Processor Scripts
./stopProcessor
./startProcessor

## Process Group Scripts
./stopProcessGroup <processGroupUUID>
./startProcessGroup <processGroupUUID>

## Migration Scripts
In order to migrate a processGroup from one environment to the next you have to:
* generate a template of the process group (in the first environment)
* upload the template to git (in the first environment)
* upload the template to nifi (in the second environment)

./generateTemplate <processGroupUUID>
NOTE: uploadGit will only work if the proper credentials are stored in the config file
./uploadGit