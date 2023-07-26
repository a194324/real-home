<template>
  <nav aria-label="Page navigation example">
    <ul class="pagination d-flex justify-content-center">
      <li class="page-item kg"><a class="page-link" href="#">Previous</a></li>
      <li class="page-item"><a class="page-link" href="#">1</a></li>
      <li class="page-item"><a class="page-link" href="#">2</a></li>
      <li class="page-item"><a class="page-link" href="#">3</a></li>
      <li class="page-item kgd"><a class="page-link" href="#">Next</a></li>
    </ul>
  </nav>
</template>
<style lang="scss">
.pagination{
  width: 1400px;

background-color: #ffffff;
}
.kg a{
  width: 109px;
height: 39px;
background-color: #e2574c;
}
.kgd a{
   width: 109px;
height: 39px;
background-color: #e2574c;
}
a{
  margin-right: 30px;
}
</style>