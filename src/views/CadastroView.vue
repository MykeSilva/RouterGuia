
<!--/*                          Aula 287 Componentes em rota 17/05/23 23:24
                                Aula 289 Parâmetros 18/05/23 00:13 */
                                Aula 290 Nested Routes 19/05/23 00:00-->

<!--(1-287)-->
<template>
    <div>
<!--(7-290)-->
        <h4>Rota Pai</h4>
        
        <input type="text" name="email" id="email" placeholder="E-mail"><br>
        <input type="text" name="nome" id="nome" placeholder="Nome"><br>
        <button>Teste!</button>
<!--(5-289)-->
        <h4>{{parametroDaRota}}</h4>

<!--(6-290) REF A ROTA FILHA (ARQUIVO index.js 6-290), EU PRECISO TER O ROUTER LINK-->
        <router-view/>
    </div>
</template>

<!--(2-289)-->

<script>

export default{
    created(){





        //console.log("Victor Lima")
/*(3-289) EU ACESSO OS PARÂMETROS DA ROTA, ATRÁVES DO OBJETO ROUTE. ESSE É UM OBJETO DE INSTÂNCIA,
EU PRECISO COLOCAR UM THIS ANTES */
        //console.log(this.$route.params.dado);
// A VARIÁVEL PARAMETRO DA ROTA VAI SER SOBRESCRITA COM OQUE EU DIGITAR NA URL (EX: victor/TESTE - victor/LIMA LIMA)
        //this.parametroDaRota = this.$route.params.dado;



    },
/*(4-289) */
    data(){
        return{
// DEFININDO UMA VARIÁVEL parametroDaRota que recebe NDA
            parametroDaRota: "Nada"
        }
    }
}

</script>