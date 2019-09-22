# Bitbucket Cloud files publisher plugin for Jenkins

On build completion, Jenkins is able to archive so-called artifacts in order to make them available from the Jenkins master server.
This plug-in provides a facility to upload these artifacts to the "Downloads" section of the BitBucket's repository.

Note: This plug-in is supported only for BitBucket Cloud solution.

## How to use the plugin

### Create a OAuth Consumer

First you need to get a OAuth consumer key/secret from Bitbucket:

1. Login into your Bitbucket account.
1. Click your account name and then in Settings from the menu bar.
1. Click OAuth from the menu bar.
1. Press the Add consumer button.
1. The system requests the following information:
1. Give a representative name to the consumer e.g. Jenkins build status notifier.
1. Although is not used, a Callback URL must be set e.g. ci.your-domain.com.
1. Leave blank the URL field.
1. Add Read and Write permissions to Repositories.
1. Click Save button and a Key and Secret will be automatically generated.

### Add OAuth Credentials to Jenkins

Add the Bitbucket OAuth Consumer credentials (as global credential for the Jenkins' instance).

1. Open Jenkins Manage Jenkins page.
1. Click Configure System.
1. Go to the section Bitbucket Build Status Notifier plugin
1. If you still don't have stored the credentials click Add, otherwise you can skip this step.
1. Select Username with password.
1. Set the the OAuth consumer key in Username.
1. Set the the OAuth consumer secret in Password.
1. Click Add button.
1. Select the desired credentials.
1. Click Save button.


