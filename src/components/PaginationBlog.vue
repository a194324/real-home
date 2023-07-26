<template>
  <nav aria-label="Page navigation example">
    <ul class="pagination d-flex justify-content-center">
      <li class="page-item kg"><a class="page-link" href="#">1</a></li>
      <li class="page-item"><a class="page-link" href="#">2</a></li>
      <li class="page-item kg"><a class="page-link" href="#">3</a></li>
      <li class="page-item kg"><a class="page-link" href="#">4</a></li>
    </ul>
  </nav>
</template>
<style lang="scss">
.pagination {
  width: 1400px;
  background-color: #ffffff;
}

.kg a {
  width: 50px;
  height: 50px;
  background-color: #e2574c;
}
.pagination a{
  width: 50px;
  height: 50px;
}


a {
  margin-right: 30px;
}</style>