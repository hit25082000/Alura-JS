﻿# Alura-JS

## Aprendizado

- Decidi automatizar o exemplo do curso como forma de me desafiar

> Implementei uma função que captura o objeto e toca o audio respectivo a seu data-id
> E um foreach com querySelectorAll que captura todos botões e atribui onclick apontando o mesmo para a função
> Assim automatizando todo o projeto do curso de JS iniciante da Alura

```sh
function Reproduzir(som){    
    let nomeSom = som.getAttribute("data-id")
    document.querySelector(`#som_tecla_${nomeSom.toLowerCase()}`).play();
}

document.querySelectorAll('.tecla').forEach(som => {
    som.setAttribute('onclick', "Reproduzir(this), console.log(this)");
});

```
