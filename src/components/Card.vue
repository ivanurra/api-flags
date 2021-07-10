<template>
  <div class="card mb-4">
      <div class="card-body">
          <h2 class="text-center">
              {{pais.name}}
          </h2>
          <p class="text-center">
              <img 
              :src="pais.flag" 
              alt="Flag" 
              style="height:170px">
          </p>
          <p class="card-text text-center" style="margin-bottom:50px;">
              <span class="badge badge-dark d-block mb-1">Name: {{pais.nativeName}}</span><br>
              <span class="badge badge-info p-3 d-block mb-1">Population: {{numeroFormato(pais.population)}}</span><br>
              <span class="badge badge-dark d-block mb-1">Capital: {{pais.capital}}</span><br>
              <span class="badge badge-dark d-block mb-1">Region: {{pais.region}}</span>
          </p>
      </div>
  </div>
</template>

<script>
export default {
    props: ['pais'],
    setup(){
        const numeroFormato = (num) => {
            return new Intl.NumberFormat("de-DE").format(num)
        }

        return {numeroFormato}
    }
}
</script>
