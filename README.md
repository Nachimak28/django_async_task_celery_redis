# A simple image thumbnailing service built using django, celery and redis as the storage backend for task queues. 

[Tutorial link](https://stackabuse.com/asynchronous-tasks-in-django-with-redis-and-celery/)

Tutorial executed in an Ubuntu 20.04 VM on GCP
## Prerequisites:

* Install conda and configure env for this app
* Install the dependencies using requirements.txt
* Install redis server in the VM [reference](https://www.digitalocean.com/community/tutorials/how-to-install-and-secure-redis-on-ubuntu-20-04)


## Notes:

* The celery worker command as given in the tutorial does not work, do the following instead
```sh
celery -A image_parroter worker --loglevel=info
```