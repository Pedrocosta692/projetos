<template>
<div class="conversor"> 
 <h2>{{moedaA}} Para {{moedaB}}</h2>
 <input type="text" v-model="moedaA_value" v-bind:placeholder="moedaA">
 <input type="button" value="Converter" v-on:click="converter">
 <h2>{{moedaB_value}} </h2>
 </div>
</template>

<script>
export default {
  name: "MeuConversor",
  props: ["moedaA", "moedaB"],
  data(){
      return{
          moedaA_value: "",
          moedaB_value: 0
      };
  },
  methods:{
      converter(){
          let de_para = this.moedaA + "_" + this.moedaB; 
          let url = "https://free.currencyconverterapi.com/api/v5/convert?q="+
             de_para +
            +"L&compact=y";
          fetch(url)
          .then(res=>{
              return res.json();
              })
          .then(json=>{
            let de_para = this.moedaA + "_" + this.moedaB;
              let cotacao = json [de_para].val;
              this.moedaB_value = (cotacao * parseFloat(this.moedaA_value)).toFixed(
                  2
              );
          });
      }
  }
  };
</script>

<style scoped>
</style>