# rappel 

```js
// fonction

// définition

// une variable permet de stocker une ou plusieurs valeurs
// une fonction permet de stoker un ou plusieurs traitements 

let a = 2 ; 

function b(){
    let a = 10 ;
    let b = 30 ;
    let c = a + b ; 
    if(){}
    for(){}
    console.log();
}

// on veut exécuter les traitements stockés dans une fonction
// il faut APPELER / EXECUTER cette fonction

b(); // EXECUTION

// quand on a besoin d'une fonction dont les traitements sont les mêmes MAIS les valeurs à porter à ces traitements sont différents => remplacer les variables dans les fonctions PAR des PARAMETRES


function c( a, b ){
    // let a = 10 ;
    // let b = 30 ;
    let c = a + b ;
}

c( 33 , 55 );
c( 52 , 24 ) ;

// si le concept de paramètre n'existait pas 


function c1(){
    let a = 33 ;
    let b = 55 ;
    let c = a + b ;   
}

function c2(){
    let a = 52 ;
    let b = 24 ;
    let c = a + b ;   
}


// return
// mot clé que l'on trouve dans les fonctions 

// à quoi ça sert ?? 

function creer_profil_etudiant( prenom , nom , age )
{
    let profil = prenom  + nom + age 
    let profil = prenom + " " + nom + " " + age 
    // prenom = "Alain"
    // nom = "DUPONT"
    // age = 22
    // profil = "AlainDUPONT22"  
    // profil = "Alain DUPONT 22" 

    // la variable porfil est LOCALE 
    return profil ; 
    // pouvoir récupérer la valeur stockée dans la variable local profil à l'extérieur de la fonction
}

// profil // ERREUR variable INCONNUE ?? 

let etudiant1 = creer_profil_etudiant("Alain" , "DUPONT" , 22) ; 
```