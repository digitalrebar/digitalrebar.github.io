README
======

To generate new files....

Get the slack log, copy the community slack json into the right community folder(s) under /slack

Remember to update the channels.json file with the renamed community folder!

From the site root, 

sudo docker run -ti --rm -v ~/digitalrebar/digitalrebar.github.io/slack:/mnt/slack_data -v ~/digitalrebar/digitalrebar.github.io/slack:/mnt/slack2html/ php:7 bash -c 'cd /mnt/slack_data && php slack2html.php'

Update the index2.html file to include the new community diretory

If you are updating an existing month, delete the HTML file for that month!

You'll need to update and replace the slack/html/index.html using slack/index2.html as a template

Also, check permissions/ownership of files!

Please check in the source json files too.