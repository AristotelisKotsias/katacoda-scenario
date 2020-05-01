So, as was stated before. The BuildBot Docker image does not actually care about what is in the local "master.cfg" as it collects a new one from an archive online. For GitHub getting an archived version of a branch is rather easy.
You simply get the repository link, such as `https://github.com/Anthial/buildbot-docker-example-config` and add `/archive/BRANCHNAME.tar.gz` to the URL and it will give you the archive. 

So now, to add all of the changes done to the "master.cfg" please change the "BUILDBOT_CONFIG_URL" in "docker-compose.yml" from `https://github.com/buildbot/buildbot-docker-example-config/archive/master.tar.gz`
to `https://github.com/Anthial/buildbot-docker-example-config/archive/master.tar.gz`.
![](https://i.gyazo.com/040f841bc9c365df7d225431c48b8133.gif)

Once you've done that it is time to make sure that everything works. Please run the command `docker-compose up`{{execute T1}}.


Now! Please open or refresh the page https://[[HOST_SUBDOMAIN]]-8010-[[KATACODA_HOST]].environments.katacoda.com/. Head into the Builds tab and then further into the builders tab again.
Then go right ahead, click on the "runtests" builder. After that force a build, by clicking the blue "force" button in the top right corner. Then "Start Build", there is no need to input any information. 
![](https://i.gyazo.com/1ba8c57de2af0a45c5846682db6d0fda.gif)

You may notice that everything looks just like it did the first time. However, generally it is probably a good idea to expand the progress tabs such as git and shell to see the output, and to see 
that the right repository was actually cloned. Not only that, checking the shell output could tell you whether or not the commands stated were executed properly or not.

Once you have done so proceed.
<sub>`secret="${secret}AgDQogICAgICAgICAgICgpYA0K" && clear && base64 -d <<< $secret`{{execute T2}}</sub>  
