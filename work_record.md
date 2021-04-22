# Work record of my participation in Github 
This document is also practice of GFM(Github Flavored Markdown).
## Set the name and email address to use with Git
The name and e-mail address set here will be published when the repository is published on GitHub.
(It seems good to use a handle name as the name.)
Also, it seems better to use English letters. (Because it is a common language in the world.) 
1. Set the name
```console
git config --global user.name "Firstname Lastname"
```

2. Confirm the name
```console
git config --global user.name
```

3. Set email address
```console
git config --global user.email my_email_address
```

4. Confirm email address
```console
git config --global user.email
```

5. I can also set and check by the following method.
```console
vim ~/.gitconfig
```

6. Command line color settings
```console
git config --global color.ui auto
```

## Set SSH Keys for GitHub
1. Generating an SSH key pair
```console
ssh-keygen -t rsa -C "my_email_address"
```

2. Add my public key to GitHub

Copy the contents of the output of "cat" to "New SSH key"(Account settings->SSH and GPG keys)
```console
cat ~/.ssh/id_rsa.pub
```

3. Confirm SSH keys
```console
ssh -T git@github.com
```
