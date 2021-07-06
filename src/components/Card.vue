<template>
  <div class="card">
      <div class="card-body">
          <h5>
              {{pais.name}}
          </h5>
          <p class="card-text">
              <span class="badge badge-dark d-block mb-1">Name: {{pais.nativeName}}</span><br>
              <span class="badge badge-info p-3 d-block mb-1">Population: {{pais.population}}</span><br>
              <span class="badge badge-dark d-block mb-1">Capital: {{pais.capital}}</span><br>
              <span class="badge badge-dark d-block mb-1">Region: {{pais.region}}</span>
          </p>
      </div>
  </div>
</template>

<script>
export default {
    props: ['pais']
}
</script>
