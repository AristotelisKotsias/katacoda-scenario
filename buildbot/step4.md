The first thing you will have to do is to configure the "docker-compose.yml" file to appropriately reference the KataCoda-version of a localhost. 
You will find the file in your editor by expanding "buildbot-docker-example" and then expanding the "simple" folder. 

If you click on the file it will open in the editor. There is only one thing you need to change here and that is the BUILDBOT_WEB_URL. It is currently set to http://localhost:8010/,
something that would work during a local installation. However the KataCoda environment is not a local environment, so you have to set the BUILDBOT_WEB_URL to the equivalent of a local environment in KataCoda. 
Replace http://localhost:8010/ with https://[[HOST_SUBDOMAIN]]-8010-[[KATACODA_HOST]].environments.katacoda.com/

Then head over to the next section. 