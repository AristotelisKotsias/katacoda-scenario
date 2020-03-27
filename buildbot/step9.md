We then start looking to the Builders category, [INSERT MORE INFORMATION HERE ABOUT BUILDERS] in particular it is interesting to look at the BuildFactory and the steps added to it. 
The first steps sets a repository to collect and the second states that a command should be executed.
So if you want to use a personal repository, you would have to replace the information `repourl='http://github.com/buildbot/pyflakes.git'` with something like `repourl='http://github.com/YOURUSERNAME/YOURREPOSITORY.git'`.
If this does not satisfy your curiosity about Builders or BuildFactories please checkout the [Builders documentation](https://docs.buildbot.net/latest/manual/configuration/builders.html) 
or the [BuildFactory documentaiton](https://docs.buildbot.net/latest/manual/configuration/buildfactories.html).

In our case, we're going to replace the repository URL `http://github.com/buildbot/pyflakes.git`with the URL `https://github.com/Anthial/pythonfun.git`. Then we are going to change the command execution in the second step from 
`command=["trial", "pyflakes"])` to `command=["python", "testpy.py"])`.

Congratulations, you've now successfully ran BuildBot's Docker image, and you've reconfigured it to utilise a different Git repository. 

Please move on to the next step.
