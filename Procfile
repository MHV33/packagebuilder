web: gunicorn packagebuilder.wsgi --log-file=- --workers $WEB_CONCURRENCY
worker: celery -A buildpackage.tasks worker -B --loglevel=debug --without-mingle --without-gossip
