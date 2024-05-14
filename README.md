# blog.nubitlan.com

#### Command used for certificate
sudo certbot certonly --manual --preferred-challenges dns -d nubitlan.com -d www.nubitlan.com

##### allowed access to cert with this
sudo chmod 755 /etc/letsencrypt/live/ /etc/letsencrypt/archive/
sudo chmod 644 /etc/letsencrypt/live/nubitlan.com/fullchain.pem
sudo chmod 644 /etc/letsencrypt/live/nubitlan.com/privkey.pem

#### Add metadata and scripts with:
docker exec -it [container-ID] bash
nano /var/www/html/wp-content/themes/[your-active-theme]/header.php