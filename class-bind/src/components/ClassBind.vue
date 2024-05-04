<template>
    <div>
        <h1>Welcome Oscar Danilo</h1>
  <span v-bind:class="{'danger':hasError}">El mensaje se ha enviado satisfactoriamente</span> <br> <br>

  <span :style="{backgroundColor:'pink',color:currentColor}">El mensaje se ha enviado satisfactoriamente</span> <br>
  
  <hr>
        <button @click="handleClick()">
            Cambiar color
        </button>
    </div>

</template>

<script lang="ts">

    import { defineComponent } from 'vue';
    import { ref } from 'vue';
    
        export default defineComponent({
            name:'ClassBind',

            setup(){

                let hasError = true;
                let alterColor = "#FFFF00";
                let firtsColor = '#000000';
                let currentColor = ref(firtsColor);

                const handleClick = ()=>{

                    currentColor.value = currentColor.value === firtsColor ? alterColor : firtsColor;
                } 
                
                return {hasError,
                    currentColor,
                    handleClick,
                    firtsColor};
                

            },

            

        })

</script>

<style scoped>
.danger{
color: red;
}
</style>