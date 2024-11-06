<template >
  <div class="max-w-7xl  ">
    
      <div 
        v-for="(cancion,index) in canciones" 
        :key="index" 
        class="p-5 my-5 bg-white rounded-xl shadow-lg flex items-center  hover:shadow-2xl transition-shadow duration-300 ease-in-out"
      >
        <h1 id="NSound">{{ index +1 }}</h1>
        <span class="text-lg font-semibold ml-8">{{ cancion }}</span>
        <button 
          class=" ml-[70%] bg-blue-500 text-white py-2 px-4 rounded-full text-sm hover:bg-blue-600 transition duration-300 ease-in-out"
        >
          Reproducir
        </button>
      
    </div>
  </div>
</template>

<script>
export default {
  name: "CancionesComponent",
  data() {
    return {
      canciones: [
        "Canción ",
        "Canción ",
        "Canción ",
        "Canción ",
        "Canción ",
        "Canción ",
      ]
    };
  }
};
function contador() {
    let cant= canciones.length;
    let ex=0;
    for (let index = 0; index < cant; index++) {
      ex ++;
      ex.innerText=Nsound.toString();
    }
  }
</script>
