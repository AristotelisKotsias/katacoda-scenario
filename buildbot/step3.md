You are now ready to install the BuildBot Docker image. Do note that for this tutorial we will only be modifying the standard BuildBot image. 
If you were to do this on a local installation, the recommendation would be to fork [this](https://github.com/buildbot/buildbot-docker-example-config) GitHub repository, 
to allow you to modify it as you see fit (and to allow you to save your BuildBot configuration). More on forking GitHub repositories can be found [here](https://help.github.com/en/github/getting-started-with-github/fork-a-repo)

Time to get the necessary files! Please run `git clone --depth 1 https://github.com/buildbot/buildbot-docker-example-config`{{execute HOST1}} to clone the GitHub BuildBot Docker image. 

Once this is done, please head into the folder where the Docker image is. If you haven't changed the cloning command above, you should run `cd buildbot-docker-example-config/simple`{{execute HOST1}}

After that, it would just be a matter of running the image using `docker-compose up`, if you were doing this on a local installation. However, this Tutorial takes place in a KataCoda environment.
Therefore the BuildBot image has to be configured appropriately. More on that in the next section. 
