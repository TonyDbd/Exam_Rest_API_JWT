# Exam_Rest_API_JWT
CRUD via API Platform avec Authentification Jwt

    php bin/console doctrine:fixtures:load 
Charge Les ravioles & les users


# Via Postman
Inscription: 
method POST     http://localhost:8000/register

{ "email": "admin@admin.com", "password": "admin" }

login: 
method POST     http://localhost:8000/login_check
{ "username": "admin@admin.com", "password": "admin" }

Token créé ! 
copier / coller { Authorization → Type = Bearer Token }

method get      http://localhost:8000/api/ravioles 
                http://localhost:8000/api/ravioles/1

method put      http://localhost:8000/api/ravioles/1

method delete   http://localhost:8000/api/ravioles/1
