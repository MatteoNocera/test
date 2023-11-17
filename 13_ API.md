# Rotte API

```php
Rooute::get('posts', function() {
    return[
        'status' => 'success',
        'result' => 'Ciao API Laravel'
    ];
})
```

![Alt text](image-529.png)

![Alt text](image-530.png)

![Alt text](image-531.png)

![Alt text](image-532.png)

![Alt text](image-533.png)

![Alt text](image-534.png)

![Alt text](image-535.png)

![Alt text](image-536.png)

![Alt text](image-537.png)

![Alt text](image-538.png)
Se non metti nulla pagina a 15 risultati

![Alt text](image-539.png)

![Alt text](image-540.png)

![Alt text](image-541.png)

![Alt text](image-542.png)

![Alt text](image-543.png)

```bash
npm install axios
```

![Alt text](image-544.png)

![Alt text](image-545.png)

npm i --save bootstrap @popperjs/core

npm i --save-dev sass

- rinomina il file style css in scss
importa bootstrap @use "../node_modules/bootstrap/scss/bootstrap.scss"

- in main js cambia il nome in scss

![Alt text](image-546.png)

![Alt text](image-547.png)
admin non login

![Alt text](image-550.png)
mi imposto la mia base url

![Alt text](image-551.png)

![Alt text](image-552.png)

- Sul seeder si possono assegnare i post all'utente con id 1

![Alt text](image-553.png)
![Alt text](image-554.png)

- pagination
![Alt text](image-555.png)

![Alt text](image-556.png)

## CORS POLICY
- su 'allowed_origins' => ['*']
permetto le origini da qualsiasi dominio o app, potenzialmente milioni di richieste.
![Alt text](image-557.png)
- Se il dominio non è consentito la richiesta non va a buon fine con un http CORS error
![Alt text](image-558.png)

![Alt text](image-559.png)

- possiamo inserire i domini nell'array

![Alt text](image-560.png)

![Alt text](image-561.png)

- Creo variabile in .env e in .env.example
![Alt text](image-562.png)

![Alt text](image-563.png)

![Alt text](image-564.png)

![Alt text](image-565.png)

![Alt text](image-567.png)
php artisan db:seed --class=ProjectSeeced