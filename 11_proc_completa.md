# Procedura Laravel con Laravel Breeze

![Alt text](image-427.png)

https://laravel.com/docs/10.x/starter-kits#laravel-breeze

- laravel new "nome progetto"

- composer require laravel/breeze --dev

- imposto nel file .env i valori giusti per entrare nel db

- php artisan breeze:install (scegli blade, no e Pest)

- php artisan serve

- composer require pacificdev/laravel_9_preset

- php artisan preset:ui bootstrap --auth

- change js in cjs

- npm i

- npm run dev

- cancella guest ed edit dentro le view

- php artisan migrate

- php artisan make:controller Admin/DashboardController

(inserisco index al suo interno che mi return view alla admmin dashboard)
(aggiungo admin a views e ci inserisco dashboard)
(modifico nella web la rotta gestendo con il controller)

![Alt text](image-428.png)

(modifico il gruppo di rotte)

![Alt text](image-429.png)

(modifico le rotte con ->prefix('admin'))

![Alt text](image-430.png)

Finale

![Alt text](image-431.png)

![Alt text](image-432.png) Aggiungo il nome iniziale

### Ultima
![Alt text](image-434.png)

- cambio in providers il providers service per cambiare il nome della rotta

![Alt text](image-433.png)

- copio la app.blade e la nuova la rinomino in admin.blade e la modifico
(posso prendere spunto dagli esempi di dashboard di bootstrap o dal layout di Fabio)

- collego file sistem in public e in config file sistem in public

- php artisan storage:link

- php artisan make:model Post -a        (ci fa policy e factory oltre a seeder e resources e controller che sposteremo in admin modificando il percorso e importando i controller)

- cancello le policy

- popolo la tabella delle migrazioni
- ![Alt text](image-436.png)
- Slug ![Alt text](image-439.png)

- entro nel seeder per compilare i dati
- ![Alt text](image-438.png)

- DatabaseSeeder
- ![Alt text](image-437.png)

- php artisan migrate

- php artisan db:seed

- se metto una image con faker creo una cartella dedicata placeholders:
-  ![Alt text](image-441.png)
- ## Attenzione : potrebbe non funzionare

- php artisan ti 
(App\Models\Post::all())

- su web inserisco le rotte resource
- ![Alt text](image-442.png)
- php artisan route:list

- implemento il controller lato admin
- ![Alt text](image-443.png)

- dentro admin aggiungo la cartella dei posts e inserisco le rotte resource (index create ecc)

- su admin.posts.index implemento la view con l'estensione del layout e la section content stampando poi i miei post
- ![Alt text](image-444.png) ![Alt text](image-445.png)

- recupero le immagini
- ![Alt text](image-446.png)

- ### Pagino i risultati
- php artisan vendor:publish (cerco laravel-pagination)
- ![Alt text](image-447.png)
- ![Alt text](image-448.png)

- per richiamare il post tramite lo slug e non l'id come di default uso:
- ![Alt text](image-449.png)

- su StorePostRequest authorize return true
- ![Alt text](image-452.png)
-- ![Alt text](image-453.png)

- implemento la create
- ![Alt text](image-450.png)
- creo la view come al solito con all'interno il form
- ![Alt text](image-451.png)
- validate
- ![Alt text](image-454.png)


- implemento il metodo store
- validate
- ![Alt text](image-455.png)
- use Str
- ![Alt text](image-456.png)
- ## Post::created
- aggiungo il messaggio di creazione su index
- ![Alt text](image-457.png)
- nel modello aggiungo le fillable
- ![Alt text](image-458.png) ($fillable)

- aggiungo la cartella guest sulle views e posso inserire la welcome page