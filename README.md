### This is API which send the event based emails to the employee of the company

> ####  The API is developed by using DjangoREST Framework.
> ####  The API contains the base-authentication system to varify the user.
> #### The admin has a special access tho the database who can perform all operations on DB.


To use external notifications make sure to update your project `urls.py` to add a valid path for notifications

```
urlpatterns = [
    ...
    path(
        'api/event_email_sender_app/', include(('event_email_sender_app.urls', 'event_email_sender_app'), namespace='event_email_sender_app')
    ),
    ...
]
```
