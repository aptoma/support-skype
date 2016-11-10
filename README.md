Project url: https://console.cloud.google.com/code/develop/browse/default/master?project=helpdesk-skype


checkout from gcloud console: 

    gcloud config set project helpdesk-skype   && gcloud source repos clone default  ~/src/helpdesk-skype/default && cd ~/src/helpdesk-skype/default && git checkout master

test:

    dev_appserver.py --php_executable_path=/usr/bin/php-cgi $PWD

deploy:

    gcloud app deploy app.yaml

open app on the web from console: gcloud app browse 
web: https://helpdesk-skype.appspot.com
