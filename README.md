# threadfix
# Get Application Metadata ID
curl --insecure -H 'Accept: application/json' -H "Authorization: APIKEY 0le3ZkV70eYtFXazIWFLgQx0VgMcBTrDQPbJasm0NFw" http://vsoc.mooo.com:9280/threadfix/rest/metadataKeys?type=Application

# Update Application Metadata 
curl --insecure -H 'Accept: application/json' -H "Authorization: APIKEY 0le3ZkV70eYtFXazIWFLgQx0VgMcBTrDQPbJasm0NFw" -X POST --data description=Pass http://vsoc.mooo.com:9280/threadfix/rest/applications/7/metadata/1/update

curl --insecure -H 'Accept: application/json' -H "Authorization: APIKEY 0le3ZkV70eYtFXazIWFLgQx0VgMcBTrDQPbJasm0NFw" -X POST --data description=N/A http://vsoc.mooo.com:9280/threadfix/rest/applications/7/metadata/2/update

curl --insecure -H 'Accept: application/json' -H "Authorization: APIKEY 0le3ZkV70eYtFXazIWFLgQx0VgMcBTrDQPbJasm0NFw" -X POST --data description=N/A http://vsoc.mooo.com:9280/threadfix/rest/applications/7/metadata/3/update

# Delete Application Metadata key value --> Caution, If you delete metadata the id will be change 
curl --insecure -H 'Accept: application/json' -H "Authorization: APIKEY 0le3ZkV70eYtFXazIWFLgQx0VgMcBTrDQPbJasm0NFw" -X DELETE http://vsoc.mooo.com:9280/threadfix/rest/applications/7/metadata/3/delete

# Get Application Metadata
...

