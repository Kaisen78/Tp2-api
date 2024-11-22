# Tp2-api

## Étape 1 : Requête GET sur les comments  
### Requête  
**Méthode :** `GET`  
**URL :** `https://jsonplaceholder.typicode.com/comments`

### Résultat attendu  
Récupère tous les commentaires disponibles dans l'API.

---

## Étape 2 : Requête POST sur les todos  
### Requête  
**Méthode :** `POST`  
**URL :** `https://jsonplaceholder.typicode.com/todos`  
**Headers :**  
- Content-Type: `application/x-www-form-urlencoded`

**Body (x-www-form-urlencoded) :**  
| Key       | Value         |  
|-----------|---------------|  
| userId    | 1             |  
| title     | Learn APIs    |  
| completed | false         |  

### Résultat attendu  
Un nouvel objet `todo` est créé avec les paramètres spécifiés.

---

## Étape 3 : Requête PATCH sur les posts  
### Requête  
**Méthode :** `PATCH`  
**URL :** `https://jsonplaceholder.typicode.com/posts/1`  
**Headers :**  
- Content-Type: `application/json`

**Body (raw, JSON format) :**  
```json
{
  "title": "Updated Title",
  "body": "Updated Body Content"
}
```

### Résultat attendu  
L'objet `post` avec l'identifiant `1` est mis à jour avec un nouveau `title` et un nouveau `body`.

---

## Étape 4 : Requête GET pour afficher les commentaires associés au post avec l’identifiant 1  
### Requête  
**Méthode :** `GET`  
**URL :** `https://jsonplaceholder.typicode.com/posts/1/comments`

### Résultat attendu  
Récupère tous les commentaires associés au post avec l'identifiant `1`.

---

## Étape 5 : Requête GET pour afficher les photos associées à l’album numéro 2  
### Requête  
**Méthode :** `GET`  
**URL :** `https://jsonplaceholder.typicode.com/albums/2/photos`

### Résultat attendu  
Récupère toutes les photos associées à l'album ayant l'identifiant `2`.
