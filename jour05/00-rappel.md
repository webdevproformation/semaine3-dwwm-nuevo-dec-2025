# rappel 


ajouter une image dans une page html

```html
<img src="https://placehold.co/400x150" alt="">
source = src
```

MDN : Modzilla Developer Network => Larousse / Becherelle du developpeur web 



```js
function traitement(){}
let duree = 1000 ; // durée en millisecondes 

// exécuter la fonction traitement toutes les 1 secondes (à l'infini)
let interval = setInterval(  traitement  ,  duree )

// opération inverse (stopper exécution infini)
clearInterval(interval)
```


# système d'onglet 

```html
<button>Action</button>
<button>Action</button>
<div></div>
<div></div>
```

```js
let button = document.querySelectorAll("button");
let div    = document.querySelectorAll("div");


// evenement => addEventListener

function effet( e ) 
// le paramètre e permet d'avoir des infos sur l'action que l'on vient de déclencher
{
    let index = e.target.dataset.index
    // faire l'effet escompté
}

for(let i = 0 ; i < button.length ; i = i + 1){
    button[i].addEventListener( "click" , effet )
}

```