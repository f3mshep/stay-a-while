# stay-a-while
MyBB forum for Roleplaying

# Setup
Run `docker compose up`
This will perform the following actions:
  1. Run nginx as a reverse proxy and server in a container
  2. Start a container running mybb software
  3. Start a postgres server running in a container
  4. Start the certbot script, which will handle ssl certificate signing
  
# How do I get my SSL cert again?
You will need to comment out the SSL/443 stuff in the nginx.conf and then run the `./init-letsencrypt.sh` file. 
