# Using PAT (Personal Access Token) Clone to Git with HTTP or HTTPS instead of SSH
This is only a documentation for cloning git repo using personal access token using http or https

If you have BitBucket or Git repo you have options to clone your repo using either SSH or HTTPS-PAT (Personal Access Token).

# How to use PAT
> Go to your settings -> Manage Account -> HTTP access tokens -> Create Token

When you enter screen for creating the token please select required Project Permissions. <br/>
Now you will get a personal access token something like for example <br/>
```
personalAccessToken = perNzAyODYxMzQ5MTE1Ossssssssssssssssssssssssss
``` 

# If you have HTTPS url
Once you have the permissions you can clone the project using the following commands.

If you have HTTP url then you can skip Step 1

### Step 1
```
git config --global http.sslVerify = false
```

### Step 2
You have to format the URL of git as shown below. 
```
git clone http://gitUsername:personalAccessToken@myBitbucketRepo.git
```

OR for example
```
git clone http://gitUsername:perNzAyODYxMzQ5MTE1Ossssssssssssssssssssssssss@myBitbucketRepo.git
```


