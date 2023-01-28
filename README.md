### tailwind 
This app uses [Django Tailwind](https://django-tailwind.readthedocs.io/en/latest/index.html).
#### Running in development mode

To start Django Tailwind in development mode, run the following command in a terminal:

`python manage.py tailwind start`

This will start a long-running process that watches files for changes. Use a combination of `CTRL + C` to terminate the process.

Several things are happening behind the scenes at that moment:

1. The stylesheet is updated every time you add or remove a CSS class in a Django template.
2. The `django-browser-reload` watches for changes in HTML and CSS files. When a Django template or CSS is updated, browser refreshes them. That gives you a smooth development experience without the need to reload the page to see updates.

#### Building for production

To create a production build of your theme, run:

`python manage.py tailwind build`

