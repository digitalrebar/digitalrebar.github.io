README
======

To generate new files....

Get the slack log, copy the community slack json into the right community folder under /slack

From the site root, 

sudo docker run -ti --rm -v ./slack:/mnt/slack_data -v ./slack:/mnt/slack2html/ php:7 bash -c 'cd /mnt/slack_data && php slack2html.php'

You'll need to update and replace the slack/html/index.html using slack/index2.html as a template
