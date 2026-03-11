# 0376RA4PR1 - Exercicis de DOM
## Contingut del repositori
- index.html
- style.css
- script.js
- README.md

## Exercicis RAEx7

1. **Selecció d’elements:** Canvia el color del `<h1>` quan la pàgina carregui.
```javascript
document.querySelector("#titol-principal").style.color = "blue";

 document.getElementById("paragraf-hola").textContent = "Hola Món";

 document.getElementById("imatge-canviant").setAttribute("src", "nova-imatge.jpg");

 document.getElementById("caixa-estil").addEventListener("click", function(){
    this.style.backgroundColor = "lightblue";
});

document.getElementById("boto-toggle").addEventListener("click", function(){
    document.getElementById("text-classe").classList.toggle("actiu");
});

document.getElementById("boto-alerta").addEventListener("click", function(){
    alert("Has clicat el botó!");
});

document.getElementById("boto-afegir").addEventListener("click", function(){
    let li = document.createElement("li");
    li.textContent = "Nou producte";
    document.getElementById("llista-compra").appendChild(li);
});

document.getElementById("element-eliminar").addEventListener("click", function(){
    this.remove();
});
