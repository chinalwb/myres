# pact-sdui-client-android
Android apps for SDUI clients

We will maintain all of the Pact SDUI client apps in this repository.


## Authenticating to build the app
_Because this app depends on our [Pact SDUI private library](https://github.com/martingalecorp/pact-sdui-poc-android/packages/915327), we'll need authenticate ourselves for downloading the packages._

1. Go to GitHub Settings and generate a new Personal Access Token.
2. Endow it with read:packages scopes.
<img width="773" alt="read_packages" src="https://user-images.githubusercontent.com/1758864/127301630-815a1056-bded-4543-9d38-b6160822fc1e.png">


3. Copy on your clipboard the generated token 
4. On Mac, issue this command: `open ~/.gradle/gradle.properties` (or just go to Finder and edit this file)
5. Append these two lines at the end of the file: 
```
GITHUB_USER=your_github_username
GITHUB_PERSONAL_ACCESS_TOKEN=paste_the_PAT
``` 
6. Check the repo out and now you will be able to download the package and build the app
