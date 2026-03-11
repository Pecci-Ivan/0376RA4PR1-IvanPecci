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

3. **Modificar atributts:** Canvia la imatge amb `serAttribute`.

 document.getElementById("imatge-canviant").setAttribute("src", "imatge.jpg");

4. **Estils:** Canvia el color de fons d´una caixa amb `backgroundColor`.

 document.getElementById("caixa-estil").addEventListener("click", function(){
    this.style.backgroundColor = "lightblue";
});

5. **Classes:** Afegir o treure una classe amb classList.toggle.

document.getElementById("boto-toggle").addEventListener("click", function(){
    document.getElementById("text-classe").classList.toggle("actiu");
});

6. **Esdeveniments:** Mostra una alerta en fer clic a un botó.

document.getElementById("boto-alerta").addEventListener("click", function(){
    alert("Has clicat el botó!");
});

7. **Crear i afegir elements:** Afegir un nou `<li>` a la llista.

document.getElementById("boto-afegir").addEventListener("click", function(){
    let li = document.createElement("li");
    li.textContent = "Nou producte";
    document.getElementById("llista-compra").appendChild(li);
});

8. **Eliminar elements:** Fer que un element desaparegui al fer clic.

document.getElementById("element-eliminar").addEventListener("click", function(){
    this.remove();
});
