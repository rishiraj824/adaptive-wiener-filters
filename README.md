### Locally Adaptive Wiener Filters

This [demo](https://github.com/rishiraj824/adaptive_wiener_filters/blob/master/demo/WienerFilters.ipynb) discusses
denoising using locally adaptive Wiener Filters.

##### Requirements to run this app: python3, cv2, numpy, whitenoise

To run the Django app, run the following steps:

- `git clone https://github.com/rishiraj824/adaptive_wiener_filters.git`
- `python manage.py makemigrations`
-  `python manage.py migrate`
- `python manage.py createuser`
- `python manage.py runserver`
- Login here with the credentials, http://127.0.0.1:8000/admin

Open Postman to use the following API:

```
curl --location --request POST 'http://127.0.0.1:8000/upload' \
--header 'Content-Type: multipart/form-data' \
--header 'Cookie: csrftoken=2cOkPfRynq7rfYClEITWDBovmvOjeOtuqtcJvkx0caMyrWoDvNJDaX6pbbaafclo' \
--form 'image=/path/to/image.jpg' \
--form 'name=blur.jpg'
--form 'color=false'
```