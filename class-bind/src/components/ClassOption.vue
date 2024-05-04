<template>

        <h1>nuevo cliclo de vida del componete con option A.P.I</h1>
</template>


<script lang="ts"  >
    import { defineComponent } from 'vue';

    export default defineComponent({

            name:"ClassOption",

            data() {
                return {
                    
                }
            },
            methods: {
                
            },
            created(){
                console.log('CREATED');
                
            },
            mounted() {
                console.log('MOUNTED');
                
            },
            updated() {
                console.log('UPDATE');
                
            },
            unmounted() {
                console.log('unmounted');
                
            },





    })

</script>