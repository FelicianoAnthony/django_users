## Django REST -- user login, create new users, passsword reset 

(( create venv && pip install django djangorestframework))
## this is for admin 

` http://127.0.0.1:8000/accounts/login/ to login with superuser credentials 

 - home.html gets displayed when you login 

 - home.html has a logout button (can also go to http://127.0.0.1:8000/admin/ to logout in upper right corner )

 - when you go back to http://127.0.0.1:8000/ you will be logged out 

https://wsvincent.com/django-user-authentication-tutorial-login-and-logout/

`


## register new users 

`
 http://127.0.0.1:8000/accounts/signup/ (signup.html) -- to register a new user 
 

 - then will be redirected to http://127.0.0.1:8000/accounts/login/ (login.html) - where you login w/ new account 


 - then redirected to http://127.0.0.1:8000/ (home.html) 


https://wsvincent.com/django-user-authentication-tutorial-signup/
`


## reset password 


`
http://127.0.0.1:8000/accounts/password_reset/ (password_reset_form.html) -- send "fake email" -- takes you to http://127.0.0.1:8000/accounts/password_reset/done/ (password_reset_done.html)

- for this tutorial -- use admin@example.com since that email already exists -- need to add something to send message if email address doesn't exist 

- go to sent_emails folder, open log file, & copy url that looks like http://127.0.0.1:8000/accounts/reset/MQ/4yb-b75404d0e53c6e4cd104/ then it takes you to http://127.0.0.1:8000/accounts/reset/MQ/set-password/ where you can reset password then login 

https://wsvincent.com/django-user-authentication-tutorial-password-reset/

`