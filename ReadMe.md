# Step - 1

    create a service account from the firebas console
    project settings -> service accounts -> generate new private key

# Step - 2

    copy code fom the downloaded json file to appConfig.json file

# Step - 3

    Run this command

```bash
    npx -p node-firestore-import-export firestore-export -a appConfig.json -b backup.json
```

# Step - 4

    backup.json file will be created in the root directory of the project where the export of your db can be found

# Step - 5

    Run this command, to import the data back to the firestore db fo another project

```bash
    npx -p node-firestore-import-export firestore-import -a appConfig2.json -b backup.json
```
