## Part 2 - Setup Load Balancing TODOs

Setup the following and add documentation or screenshots to your `README.md` file as specified.

1. Create an `/etc/hosts` OR `.ssh/config` file on each system that correlates hostnames to private IPs.
   - I edited /etc/hosts to add the webserv IP's.
   - ![Part 2 1 5668](https://user-images.githubusercontent.com/77283021/159066182-4a7c7951-3252-407a-a2e2-2b4e9048acb7.png)
2. Document how to SSH in between the systems utilizing their private IPs.
      - Once you are in your Proxy Instance. You want to use the following command style "ssh -i yourkeyname servername". 
3. **_HAProxy configuration & documentation requirements_**
   - How to set up a HAProxy load balancer
     - What file(s) where modified & their location
         - /etc/haproxy/haproxy.cfg
     - What configuration(s) were set (if any)
         - ![2 3](https://user-images.githubusercontent.com/77283021/159068650-ddf32e06-062b-420b-98ff-43c5a033e5ca.png)
     - How to restart the service after a configuration change
         - "sudo systemctl restart haproxy"
4. **_Webserver 1 & 2 configuration & documentation requirements_**
   - How set up a webserver
     - What file(s) were modified & their location
          - /var/www/html/index.html was modified
     - What configuration(s) were set (if any)
          - No configurations set
     - Where site content files were located (and why)
          - Location is /var/www/html
          - Located here because of apache2 having this set as the default location to pull from.
     - How to restart the service after a configuration change
          - sudo systemctl restart apache2

5. From the browser, when connecting to the proxy server, take two screenshots.
   - one screenshot that shows content from "server 1"
            - ![server1](https://user-images.githubusercontent.com/77283021/159075565-7577690e-04e8-4602-93d2-149345507059.PNG)
   - one screenshot that shows content from "server 2"
            - ![Server2](https://user-images.githubusercontent.com/77283021/159075569-3295e3eb-690c-4b7c-99e6-0b8d4a4bd0e7.PNG)

6. Resources used for Project 3
   - Lecture Recordings
   - Lecture notes
   - https://www.haproxy.com/blog/the-four-essential-sections-of-an-haproxy-configuration/
      - As used in class
