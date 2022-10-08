# python packages

## start

```bash
python3 manage.py runserver 0.0.0.0:8000
```

## install

!pip freeze > requirements.txt

!pip install .

```bash
!pip install -e .
```

How to Get the Requirements.txt File: Using Virtualenv

To create the requirement.txt file, we can use the following command:
all packages in env

```bash
pip3 freeze > requirements.txt
```


If you created a Python requirements.txt file at one point but have failed to maintain it for some reason

```bash
pip list --outdated .
```


Install from 
```bash
pip install -r requirements.txt
```

to use the pipreqs module. It is used to scan your imports and build a Python requirements file for you.
```bash
pip install pipreqs  
pipreqs /path/to/project
pipreqs .
pipreqs src
```

to check for missing dependencies, you can do so with the following command:
```bash
python3 -m pip check
```

How to Get the Requirements.txt File: Using Pipenv
```bash
pip install pipenv
```

```bash
pipenv install mypackage
```

GENERATE
```bash
pipenv run Python main.py   
pipenv -r lock >> requirements.txt
```

[Install Docker Engine on Ubuntu | Docker Documentation](https://docs.docker.com/engine/install/ubuntu/#set-up-the-repository)

> #### Set up the repository
> 
> 1.  Update the `apt` package index and install packages to allow `apt` to use a repository over HTTPS:
>     
> 
> sudo apt-get update-        sudo apt-get install \
>             ca-certificates \
>             curl \
>             gnupg \
>             lsb-release
>         
>     
> -   Add Docker’s official GPG key:
>     
> sudo mkdir \-p /etc/apt/keyrings-        curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
>         
>     
> -   Use the following command to set up the repository:
>     
> 
> 1.       echo \
>           "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
>           $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
>         
>     
> 
> #### Install Docker Engine
> 
> 1.  Update the `apt` package index, and install the _latest version_ of Docker Engine, containerd, and Docker Compose, or go to the next step to install a specific version:
>     
> 
> sudo apt-get update-        sudo apt-get install docker-ce docker-ce-cli containerd.io docker-compose-plugin
>         
>     
>     > Receiving a GPG error when running `apt-get update`?
>     > 
>     > Your default umask may not be set correctly, causing the public key file for the repo to not be detected. Run the following command and then try to update your repo again: `sudo chmod a+r /etc/apt/keyrings/docker.gpg`.
>     
> -   To install a _specific version_ of Docker Engine, list the available versions in the repo, then select and install:
>     
>     a. List the versions available in your repo:
>     
> apt-cache madison docker-ce
> 

```bash
sudo docker image build .
sudo docker images
docker run
sudo docker image prune -y
``` 