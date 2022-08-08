<template>
     <div class="container">
                    <div class="row">
                        <div class="col">
                            <div>
                                <div>
                                    <h5>
                                        Calculo de tiempo de carga:
                                    </h5>

                                    <div>
                                        <div>
                                            <div>
                                                <label for=""><small>Capacidad de Batería kwH</small></label><br>
                                                <input id="valor1" type="number">
                                            </div>
                                            <div>
                                                <label for=""><small>Potencia del cargador kW</small></label><br>
                                                <input id="valor2" type="number">
                                            </div>
                                            <div style="display: block"> <br>
                                                <button type="button" @click="calculo">
                                                    Calcular
                                                </button>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <h5>
                                Tiempo de carga: <span class="resultado"></span>
                            </h5>
                        </div>

                        <div class="col">
                            <nav class=kwh>
                                Modelos más vendidos en Chile
                                <table class="table">
                                    <thead>
                                        <tr>
                                            <th scope="col">#</th>
                                            <th scope="col">Marca</th>
                                            <th scope="col">Modelo</th>
                                            <th scope="col">Batería</th>
                                        </tr>
                                    </thead>
                                    <tbody>
                                        <tr>
                                            <th scope="row">1</th>
                                            <td>Maxus</td>
                                            <td>EV80</td>
                                            <td>56 KwH</td>
                                        </tr>
                                        <tr>
                                            <th scope="row">2</th>
                                            <td>Hyundai</td>
                                            <td>Ioniq</td>
                                            <td>28 KwH</td>
                                        </tr>
                                        <tr>
                                            <th scope="row">3</th>
                                            <td>Nissan</td>
                                            <td>Leaf</td>
                                            <td>40 KwH</td>
                                        </tr>
                                        <tr>
                                            <th scope="row">4</th>
                                            <td>MG</td>
                                            <td>ZS EV</td>
                                            <td>44.5 KwH</td>
                                        </tr>
                                        <tr>
                                            <th scope="row">5</th>
                                            <td>Porsche</td>
                                            <td>Taycan</td>
                                            <td>93.4 KwH</td>
                                        </tr>
                                    </tbody>
                                </table>
                            </nav>
                        </div>

                    </div>
                </div>
</template>
<script>
export default {
  name: 'calculadora-carga-emovi',
  props: {
  },
  methods:{
    calculo(){
    const n1= document.getElementById('valor1').value
    const n2= document.getElementById('valor2').value
    const cargaTiempo=(n1/n2)

    const horas=Math.trunc(cargaTiempo)
    const minutos=parseInt(cargaTiempo-horas)*60

    document.querySelector(".resultado").innerHTML=+horas+" horas y "+minutos+" minutos"
    }  
}
}
</script>