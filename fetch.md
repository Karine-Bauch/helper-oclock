Salut Apprenant1 !

Alors, pour ta question sur fetch.
Fetch signifie "aller chercher".

L’API Fetch c’est une interface JavaScript qui permet notamment via la méthode `fetch()` de récupérer des données `method GET` (via des requêtes http, par exemple).
Cela permet également d'envoyer des données vers le serveur via la `method POST` et d'autres (`PATCH, PUT, DELETE`).

Cela te retournera une promesse (promise) qui contient les données que tu as demandé.

Il faudra donc résoudre la promesse pour récupérer les données dont tu as besoin.
en utilisant `.then()` ou avec `async/await`.

Tu peux l'utiliser simplement en ajoutant dans ton fichier html (ou ejs), un script js qui contient la fonction fetch.

Utilisons par exemple une route que tu viens de créer dans ton parcours `http://localhost:1234/card/7` qui retourne un objet json avec les informations de la carte dont l'id est 7.

- **en utilisant `.then()`** :
```js
<script>
  fetch('http://localhost:1234/card/7')
  .then(response => console.log(response))
</script>
```

- **en utilisant `async/await`** :
```js
  <script>
    async function fetchUser() {
      const response = await fetch('http://localhost:1234/card/7');
      console.log(response)
    }
    fetchUser();
  </script>
```

Je te laisse tester cela pour mieux le comprendre, et approfondir le sujet avec l'aide de ces liens :

[MDN FETCH API](https://developer.mozilla.org/fr/docs/Web/API/Fetch_API)

[How To Use the JavaScript Fetch API to Get Data](https://www.digitalocean.com/community/tutorials/how-to-use-the-javascript-fetch-api-to-get-data)

[JavaScript Fetch API: A Beginner’s Guide](https://www.freecodecamp.org/news/javascript-fetch-api-tutorial/)