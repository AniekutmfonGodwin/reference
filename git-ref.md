## …or push an existing repository from the command line
    git remote add origin https://github.com/AniekutmfonGodwin/reference.git
    git branch -M main
    git push -u origin main

## …or create a new repository on the command line
    echo "# reference" >> README.md
    git init
    git add README.md
    git commit -m "first commit"
    git branch -M main
    git remote add origin https://github.com/AniekutmfonGodwin/reference.git
    git push -u origin main

## how to clone git repo with a particular ssh key
[goto link](https://stackoverflow.com/questions/6688655/select-private-key-to-use-with-git)

### 2
    `ssh-agent bash -c 'ssh-add ~/.ssh/id_rsa_test; git clone git@github.com:example/example-repo.git <folder name>'
`


## How to configure default ssh for a repo
[goto link](https://dev.to/web3coach/how-to-configure-a-local-git-repository-to-use-a-specific-ssh-key-4aml)