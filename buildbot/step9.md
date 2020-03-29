We then start looking to the Builders category. Essentially a Builder is responsible for creating new builds according to when a Build Requests is sent. To note is that Builders are assigned Workers and a Build Factory. 
The Build Factory sets up what steps should be executed by the Worker assigned to the Builder. In turn, it is particularly interesting to look at, since it determines what is actually going to happen, when
for example you force a build. 

The first step in the current Build Factory sets a repository to collect and the second step states that a command should be executed.

So if you want to use a personal repository, you would have to replace the information in the first step `repourl='http://github.com/buildbot/pyflakes.git'` with something 
like `repourl='http://github.com/YOURUSERNAME/YOURREPOSITORY.git'`. In our case, we're going to replace the repository URL `http://github.com/buildbot/pyflakes.git`with the URL `https://github.com/Anthial/pythonfun.git`. 
![](https://i.gyazo.com/e93f6cac32df6831fb9f547dacffd3d5.gif)

Then we are going to change the second step, a command execution from `command=["trial", "pyflakes"]` to `command=["python", "testpy.py"]`. We have now told BuildBot to run a Python script.
![](https://i.gyazo.com/ec34adf13e975c5e816ac636af7c50f8.gif)

Congratulations, you've now successfully ran BuildBot's Docker image, and you've reconfigured it to utilise a different Git repository. 
<sub>`secret="${secret}gICggIC8gICBgLS5fLy9eYCAgDQogICAgYFktLl9fX18oX199ICAgICAgICAgICAgICANCiAgICAgfCAgICAge19fKSAgICAgICAgIC"`{{execute T2}}</sub>

If your curiosity about Builders or BuildFactories has not been satisfied, please checkout the [Builders documentation](https://docs.buildbot.net/latest/manual/configuration/builders.html) 
or the [BuildFactory documentaiton](https://docs.buildbot.net/latest/manual/configuration/buildfactories.html).

Please move on to the next step.
