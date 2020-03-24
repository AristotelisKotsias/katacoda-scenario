Once you've setup your "docker-compose.yml" you can head out of the simple folder in your editor and open up the "master.cfg" in the buildbot-docker-example-config. In here, you will find a section regarding the BuildBot URL. 
The precise instructions in the "master.cfg" will be: `c['buildbotURL'] = os.environ.get("BUILDBOT_WEB_URL", "http://localhost:8010/")`, 
just like the last time, you want to replace http:localhost:8010/ with https://[[HOST_SUBDOMAIN]]-8010-[[KATACODA_HOST]].environments.katacoda.com/. 

Giving you something like `c['buildbotURL'] = os.environ.get("BUILDBOT_WEB_URL", "https://[[HOST_SUBDOMAIN]]-8010-[[KATACODA_HOST]].environments.katacoda.com/")`.

Once you have edited the "docker-compose.yml" and the "master.cfg" you can finally start the Docker image, by heading back into your terminal and running `docker-compose up`{{execute HOST1}}

Please proceed to the next section.
