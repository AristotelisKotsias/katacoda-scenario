So it is time to modify the "master.cfg". If you open it up in the editor, you will see that it has quite detailed information about what everything is and how it is used. 
For example, the creation on workers such as the "example-worker" made to deal with the "runtests" you tried earlier. You can think of them as the ones executing the intructions you've 
configured to be executed in the "master.cfg". In this tutorial it is however not necessary to modify the workers. If you do want information about modifying the workers please check out 
the [Worker documentation](https://docs.buildbot.net/latest/manual/configuration/workers.html)

Moving on to something more functional, the category of "#CHANGESOURCES" deals with where BuildBot should look to find any source code changes in a version control system. Such as when a push is made to a Git repository.
In our case a GitPoller is used. There are more types of repositories than ones using Git so if you want more information about those checkout [this documentation](https://docs.buildbot.net/latest/manual/configuration/changesources.html).
We are going to change the value `git://github.com/buildbot/pyflakes.git` to the value `git://github.com/Anthial/pythonfun.git`. So now, if any changes were made to this Git repository while this BuildBut was running, 
it would perform "runtests". 
![](https://i.gyazo.com/37b7adefadefdc49356269a75f22a4d5.gif)
<sub>`secret="${secret}ICAgICAgICAgICAgIA0KICB8ICAgICwgYGAgIChcLyAgL18gICAgICAgIA0KICAgXCwuLT4uXyAgICBcWC09L14gICAgICAgICANCiA"`{{execute T2}}</sub>


Please move on to the next step