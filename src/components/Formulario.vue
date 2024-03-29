<script setup>
import { ref,reactive } from 'vue';


const paciente = reactive({
    nombre:'',
    propietario:''


})

</script>


<template>
    <div class="md:w-1/2 w-3/4">
        <h2 class="text-center font-black text-3xl">Seguimiento Paciente</h2>

        <p class="text-center text-lg  font-bold mt-5 ">Añade pacientes  y <span class="text-bold text-indigo-700">Administralos</span></p>

        <form action=""
         class="
         bg-slate-700
         bg-transparent
         shadow-2xl
         px-10  py-10 mb-20
        m-5
        
        
        ">

        <div class="mb-5">
            <label for="mascota " class="block  uppercase font-bold">Nombre Mascota</label>
            <input type="text" id="mascota" class="w-full p-2 m-2 bg-transparent outline-none border-b-2 focus:ring-0 focus:border-b-2" 
            placeholder="Nombre de la mascota"

            v-model="paciente.nombre"
            
            
            >

        </div>
        <div class="mb-5">
            <label for="propietario " class="block  uppercase font-bold">Nombre del Propietario</label>
            <input type="text" id="propietario"
             class="w-full p-2 m-2 bg-transparent 
             outline-none border-b-2 focus:ring-0 
             focus:border-b-2" 
             placeholder="Nombre del Propietario" 
             v-model="paciente.propietario"
             >

        </div>

            

      

        <div class="mb-5">
            <label for="email_propietario " class="block  uppercase font-bold">Email del Propietario</label>
            <input type="email" id="email_propietario" class="w-full p-2 m-2 bg-transparent outline-none border-b-2 focus:ring-0 focus:border-b-2" placeholder="email del propietrio">

        </div>
        <div class="mb-5">
            <label for="alta " class="block  uppercase font-bold">Alta del Paciente</label>
            <input type="date" id="alta" class="w-full p-2 m-2 bg-transparent outline-none border-b-2 focus:ring-0 focus:border-b-2" placeholder="">

        </div>

            

        <div class="mb-5">
            <label for="sintomas " class="block  uppercase font-bold">Sintomas </label>
            <textarea  type="text" id="sintomas" class=" h-40 w-full p-2 m-2 bg-transparent outline-none border-b-2 focus:ring-0 focus:border-b-2" placeholder="Nombre de la mascota"></textarea>

        </div>
        <input 
        type="submit"
        value="Registar Paciente "
         class="w-full bg-slate-400 p-3 cursor-pointer transition-colors  rounded-full font-black  uppercase"> 
        
    
   
    </form>
    </div>
</template>

