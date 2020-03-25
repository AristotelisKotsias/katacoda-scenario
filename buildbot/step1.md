The first step to getting BuildBot running on your machine through Docker, is making sure you've got Docker installed. 
Please run  `docker --version`{{execute HOST1}}

If this does not work, please install Docker following the [appropriate installation instructions for your device](https://docs.docker.com/install/) (also useful for getting a local installation working).

This tutorial however assumes that you are running Ubuntu. Therefore you can install Docker by running `sudo apt-get update`{{execute HOST1}}
Followed by `sudo apt-get install docker-ce docker-ce-cli containerd.io`{{execute HOST1}}

`cat << "EOF" 
       _,.
     ,`` -.)
    '( _/'-\\-.               
   /,|``--._,-^|            ,     
   \_| |``-._/||          ,'|       
     |  ``-, / |         /  /      
     |     || |        /  /       
      ``r-._||/   __   /  /  
  __,-<_     )``-/  ``./  /
 '  \   ``---'   \   /  / 
     |           |./  /  
     /           //  /     
 \_/' \         |/  /         
  |    |   _,^-'/  /              
  |    , ``  (\/  /_        
   \,.->._    \X-=/^         
   (  /   ``-._//^``  
    ``Y-.____(__}              
     |     {__)           
           ()`` 
EOF`{{execute HOST1}}