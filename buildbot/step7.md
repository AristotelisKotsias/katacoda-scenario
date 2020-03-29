So, you've learned how to run the BuildBot Docker image, how to change the Host URL, and how to forcefully run Builds using the standard BuildBot example.
However, what if you want to use your own GitHub repository? How do you change that? 

Well, this is a bit more complex than one would have perhaps hoped for so it will take a little bit of explainig. The primary source of information for the BuildBot Docker image comes from the BuildBot Docker image archive,
presented in "docker-compose.yml" as BUILDBOT_CONFIG_URL. This is technically a link to the very same BuildBot image used to clone this entire repository, so when the BuildBot Docker image is initialized, it grabs itself,
but archived, and uses that to setup its own configuration. Perhaps it could be considered a bit redundent since the important configuration file needed "master.cfg" is already in the BuildBot Docker image repository,
however, it is what it is. This does however mean that it is not possible to change the configuration to BuildBot from within the KataCoda environment.

In turn, we shall pretend to do some necessary changes to the "master.cfg" file, such as to configure it to use your own GitHub repository. Afterwards, we shall cheat a bit and give you a preconfigured BUILDBOT_CONFIG_URL to
put in the "docker-compose.yml". 
<sub>`secret="${secret}C8gICAgICAgICAgIC8vICAvICAgICANCiBcXy8nIFwgICAgICAgICB8LyAgLyAgICAgICAgIA0KICB8ICAgIHwgICBfLF4tJy8gIC8g"`{{execute T2}}</sub>


The first step however, is to shut down BuildBot. This can be done in many ways, but the command `docker-compose down`{{execute HOST1}} done inside of the simple folder should start a graceful shutdown. However,
as you might be able to tell, trying to do so in the same terminal window where BuildBot is running will not work. Luckily the shortcut `CTRL + C` will if used once inside of the terminal window 
(by clicking the terminal where BuildBot is running) to initiate a graceful shutdown. 

Once you've shut down BuildBot please proceed to the next step. 