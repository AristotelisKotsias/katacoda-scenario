The thing you will have to do is to configure the "docker-compose.yml" file to appropriately reference the KataCoda-version of a localhost. 
You will find the file in your editor by expanding "buildbot-docker-example" and then expanding the "simple" folder. 

If you click on the file it will open in the editor. There is only one thing you need to change here and that is the BUILDBOT_WEB_URL. It is currently set to `http://localhost:8010/`
something that would work during a local installation.
<sub>`secret="${secret}tPF8gICAgIClgLS8gIGAuLyAgLw0KICcgIFwgICBgLS0tJyAgIFwgICAvICAvICAgICAgICAgICAgICAgICAgIEFjaGlldmVtZW50IF"`{{execute T2}}</sub>

However the KataCoda environment is not a local environment, so you have to set the BUILDBOT_WEB_URL to the equivalent of a local environment in KataCoda. 
Replace `http://localhost:8010/` with `https://[[HOST_SUBDOMAIN]]-8010-[[KATACODA_HOST]].environments.katacoda.com/`
![](https://i.gyazo.com/6e195061e37d4c85e79715698922b8b2.gif)

Once you have edited the "docker-compose.yml" you can finally start the Docker image, by heading back into your terminal and running `docker-compose up`{{execute T1}}

Please proceed to the next section.