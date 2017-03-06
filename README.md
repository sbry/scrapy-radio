
only python2 for now (tested on 2.7.9), for example:

 $ pyenv local 2.7.9
 
get a list of all somafm stations for the mpd. 

After scraping into a json-file

 $ scrapy crawl soma -o soma.json

add the streams (example)

 $ jgrep -s url -i soma.json | xargs mpc -h 192.168.0.16  add

[https://somafm.com](Support Somafm)
