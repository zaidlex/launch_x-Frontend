<template>
    <div class="pasteleria">   
        <a id="top" href="#"> </a>
        <div class="bienvenida">
            <h1>Pastelería Pantheon el panadero</h1>
            <i>"Siempre quice ser panadero." pantheon</i>
            <br>
            <img id="pantheon" alt="imagen pantheon panadero feliz" srcset="" src="@/assets/pantheon-poster.png">
        </div>
        <br>

        <!--Sabores de los pasteles-->
        <div class="sabores">
            <h3 class="title">Sabores disponibles para los pasteles por tan sólo $40.00 pesos mxn!.</h3>
            <ul class="lista">
                <li>Vainilla</li>
                <li>Chocolate</li>
                <li>Fresa</li>
                <li>Durazno</li>
                <li>Limón</li>
            </ul>
        </div>
        <br><br>

        <!--Diseños de los pasteles-->
        <div class="disenos">
            <h3 class="title" >Diseños que se les puede colocar al pastel.</h3>
            <span>Por $20.00 cada diseño.</span>
            <table class="tablaDisenos">
                <tr>
                    <td><img class="pastel" src="@/assets/LaMonarca.jpg" alt="La monarca"></td>
                    <td>La monarca.</td>
                </tr>
                <tr>
                    <td><img class="pastel" src="@/assets/RosetonAmarilloRosa.jpg" alt="Rosetón amarillo y rosa"></td>
                    <td>Rosetón amarillo y rosa.</td>
                </tr>
                <tr>
                    <td><img class="pastel" src="@/assets/Frutal.jpg" alt="Frutal"></td>
                    <td>Frutal.</td>
                </tr>
            </table>
            <br><br>
            <div>
                <button class="botonPedir" id="pedido" @click="$router.push({ path: '/ordenar' })">Hacer pedido</button>
            </div>
            <br>
        </div>
    </div>
</template>

<script>
export default {
  name: 'HomePasteleria',
  props: {
    
  },
  mounted() {
        window.scrollTo(0, 0);
    },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.pasteleria {
    margin: auto;    
}

.bienvenida {
    background-color:rgb(238,208,157,0.85);
    border-radius: 30px;
    padding: 10px;
    margin-top: 30px;
    margin-bottom: 30px;

    display:inline-block;
    margin-left:auto;
    margin-right:auto;
    text-align:center;
}

#pantheon {
    border-radius: 30px;
    border: 1px solid blue;
    padding: 5px;
    width: 196px;
    height: auto;
}

ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
td {
    font-size: 25px;
    display:inline-block;
    padding: 5px;
}
tr {
    background-color: rgb(238,208,157,0.6);
    border: 3px #E2B05A solid;
    border-radius: 25px;
    margin-top: 10px;
    margin-bottom: 10px;
    padding: 10px;
    display: block;
}

.tablaDisenos {
    padding: 20px;
    margin: auto;
}
.pastel {
    max-width: 80%;
    min-width: 40%;
    height: auto;
}

.botonPedir {
    background-color: rgb(248,211,137,0.6);
    font-size: 25px;
    border-radius: 4px;
}
</style>
