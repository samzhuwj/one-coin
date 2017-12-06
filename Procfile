daphne: daphne coinprice.asgi:channel_layer --port 8000 --bind 0.0.0.0 -v2
coin_worker: python manage.py runworker --settings=coinprice.settings -v2
celery_worker: celery -A coinprice.celeryconfig worker -l info
celery_beat: celery -A coinprice.celeryconfig beat -l info
