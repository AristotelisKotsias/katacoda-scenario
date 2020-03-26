The first step to getting BuildBot running on your machine through Docker, is making sure you've got Docker installed. 
Please run  `docker --version`{{execute HOST1}}

If this does not work, please install Docker following the [appropriate installation instructions for your device](https://docs.docker.com/install/) (also useful for getting a local installation working).

This tutorial however assumes that you are running Ubuntu. Therefore you can install Docker by running `sudo apt-get update`{{execute HOST1}}
Followed by `sudo apt-get install docker-ce docker-ce-cli containerd.io`{{execute HOST1}}

`
echo ICAgICAgIF8sLgogICAgICxgIC0uKQogICAgJyggXy8nLVxcLS4gICAgICAgICAgICAgICAKICAgLyx8YC0tLl8sLV58ICAgICAgICAgICAgLCAgICAgCiAgIFxffCB8YC0uXy98fCAgICAgICAgICAsJ3wgICAgICAgCiAgICAgfCAgYC0sIC8gfCAgICAgICAgIC8gIC8gICAgICAKICAgICB8ICAgICB8fCB8ICAgICAgICAvICAvICAgICAgIAogICAgICBgci0uX3x8LyAgIF9fICAgLyAgLyAgCiAgX18sLTxfICAgICApYC0vICBgLi8gIC8KICcgIFwgICBgLS0tJyAgIFwgICAvICAvIAogICAgIHwgICAgICAgICAgIHwuLyAgLyAgCiAgICAgLyAgICAgICAgICAgLy8gIC8gICAgICAgICAgICAgICAgICBCdWlsZGJvdCB3YXJyaW9yCiBcXy8nIFwgICAgICAgICB8LyAgLyAgICAgICAgIAogIHwgICAgfCAgIF8sXi0nLyAgLyAgICAgICAgICAgICAgCiAgfCAgICAsIGBgICAoXC8gIC9fICAgICAgICAKICAgXCwuLT4uXyAgICBcWC09L14gICAgICAgICAKICAgKCAgLyAgIGAtLl8vL15gICAKICAgIGBZLS5fX19fKF9ffSAgICAgICAgICAgICAgCiAgICAgfCAgICAge19fKSAgICAgICAgICAgCiAgICAgICAgICAgKClgCgo= | base64 -d`{{execute HOST1}}