Permissions
-----------

## freestyle-cloudfunctions or openapi-cloudfunctions middleware

When you use Convo middleware of type `freestyle-cloudfunctions` or `openapi-cloudfunctions`, you need to set up the following permissions on the GCP projecct:

### Enable Cloud Deployment Manager API

Go to your GCP project's `APIs & Services`, select `Library`, and then search for `Cloud Deployment Manager`. Click on the search result box, and you'll see the Cloud Deployment Manager API page, click on the `Enable` button.

![Cloud Deployment Manager API screen](https://github.com/cliffano/convo/raw/master/docs/permission-enable-cloud-deployment-manager-api.png "Cloud Deployment Manager API screen")

Without this enabled, you will get the following error:

```
Access Not Configured. Google Cloud Deployment Manager API has not been used in project <project> before or it is disabled. Enable it by visiting https://console.developers.google.com/apis/api/deploymentmanager.googleapis.com/overview?project=<project> then retry. If you enabled this API recently, wait a few minutes for the action to propagate to our systems and retry.
```