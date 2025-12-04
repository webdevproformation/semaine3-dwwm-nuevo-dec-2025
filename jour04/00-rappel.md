# rappeler les sujets abordés hier


```js

// tableau 

let notes = [ 1 ,2 , 5 , 6 , 10] ;
//            0  1   2

// traitement sur les tableaux

// comment récupérer une valeur du tableau 

notes[2] ; 
notes[4] ; 

// récupérer toutes les valeurs d'une tableau 

for(let i = 0 ; i < 5 ; i = i + 1)
{
 console.log(notes[i]);
}

for(let i = 0 ; i < notes.length ; i = i + 1)
{
 console.log(notes[i]);
}


// objet

let auto = {
    marque : "Peugeot",
    prix : 5000
};

let auto2 = {
    marque : "VW" ,
    prix :6000
};

auto.prix ; // 5000
auto2.marque ; 

let phrase = {
    auteur : "Victor",
    contenu : "bonjour !!" ,
    ecrire : function(){ // méthode
        let synthese = this.auteur + " a écrit " + this.contenu
        console.log(synthese) ;
    }
}

phrase.ecrire(); // exécuter une méthode stockée dans un objet 

// DOM

// Document Objet Model

// javascript va créer une variable qui s'appelle
document 
// objet qui est créé automatiquement par javascript qui contient TOUTES les balises html de la page 
// grâce à cet objet que l'on peut modifier la page web 
// sélectionner toutes les balises p
let p = document.querySelectorAll("p")

// sélectionner la 1ère balise p de la page 
p[0]
p[1]

// traitement sur les balises sélectionnées 

p[0].innerText      = "...." ;
p[0].style["color"] = "blue" ;
p[0].innerHTML      = "texte <h1>toto</h1>" 


let p = document.querySelector("p") // sélectionner le 1er p dans la page 

```

créer le fichier 01-exo.html
dans ce fichier vous avez une balise h1
puis 3 p
puis h2
puis 2 p 
avec javascript vous allez effectuer les manipulations du DOM suivantes

h1 remplir avec le texte "Start" et le mettre de couleur verte

les 3 p suivant doivent contenir le texte "lorem ipsum" taille de police 40px et couleur rose

le h2 doit contenir le texte "conclusion"

les derniers p doivent contenir le texte "bonjour <br> comment allez vous ???"