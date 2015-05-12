# OPS_tutorial
Just for learning

Steps 
  Step1 simple automated deployment (DevOps enabling):
  ---------------------------------------------------
  1. Dockerize smppsim, kannel , gproxy , monitor interface ,sender  ..
  2. Make infrastructure run using docker compose https://docs.docker.com/compose/
  3. Vagrant test to make it depolyed at aws ,laptop or digitalocean
  
  Step2 Automated scalability for single host exercise :
  -----------------------------------------------------
    make use of http://jasonwilder.com/blog/2014/03/25/automated-nginx-reverse-proxy-for-docker/ 
    make sms sender automatic send to unknown number of scalable smsboxes or gproxies , 
    
  Step2 Automatic service descovery :
  ---------------------------------
    make use of 
    http://jasonwilder.com/blog/2014/02/04/service-discovery-in-the-cloud/
    http://jasonwilder.com/blog/2014/07/15/docker-service-discovery/
    
  Step3 Plane for production
  --------------------------
