web: daphne asgi:channel_layer --port $PORT --bind 0.0.0.0 -v2
worker: python manage.py runworker -v2
celery_worker: celery -A coinprice.celeryconfig worker --beat -l info
