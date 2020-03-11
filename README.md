# Cloud Run with Cloud Build
This is an example to create a simple countinuous delivery pipeline to deploy containerized application into managed Cloud Run via Cloud Build.

## Setup Google Cloud Build

1. Go to Google Cloud Repositories and select "Add repository".
2. Select "Connect external repository".
3. Continue with setting up the correct project and git provider.

## Setup Google Cloud Build Trigger

1. Go to Google Cloud Build and select "Triggers".
2. Select "Create Trigger".
3. Select the repository that you have added earlier.
4. Select "Branch" under "Trigger Type"
5. Input "^master$" for "Branch(regex)". Cloud Build wiil be triggered when new commit is push to master branch. You may do the same for other branch
6. Select "Cloud Build configuration file (yaml or json)" under "Build configuration"
7. Create Trigger and try commit something into the git repository.