<template>
  <div class="contact2">
    <div class="container">
      <div class="row">
        <div class="contact__kg">
        <div class="col-md-4 col-sm-12">
          <div class="contact2__col ">
            <h2 class="contact2__title">Contact Info</h2>
            <div class="contact2__text">
            <p>Etiam commodo consequat egestas. Morbi at ligula nulla. Mauris bibendum mi vitae condimentum mollis. Sed sollicitudin enim vehicula, varius sapien id, consectetur posuere sem commodo.</p>
            </div>
            <h3>Real Home INC.
  ST STEPHEN'S HOUSE, COLSTON AVE, BRISTOL, BRISTOL BS1 4ST, UK</h3>
  <ul class="contact__info">
  <li class="contact2-item">telephone:<a class="contact2-link" href="#">+18006036565;</a></li>
        <li class="contact2-item">FAX:<a class="contact2-link" href="#">+18006036566</a></li>
        <li class="contact2-item">E-mail:<a class="contact2-link" href="#">mail@emolink.org</a></li>
  </ul>
          </div>
        </div>
        <div class="col-md-8 col-sm-12">
          <div class="contact3__title">
            <h2>Leave a Comment</h2>
          </div>
          <div class="contact-form">
  <div class="input-group mb-4">
    <input type="text" class="form-control" placeholder="Username" aria-label="Username">
    <span class="input-group-text"></span>
    <input type="text" class="form-control" placeholder="Server" aria-label="Server">
  </div>

  <div class="input-group">
    <span class="input-group-text"></span>
    <textarea class="form-control" aria-label="With textarea"></textarea>
  </div>
          </div>
          <button type="button" class="btn btn-danger ld">Danger</button>
          <button type="button" class="btn btn-light ld">Light</button>
        </div>
      </div>
      </div>
    </div>
  </div>
</template>


<style lang="scss">
.contact__kg{
  display: flex;
}
.contact2__text{
  font-family: Raleway;
font-size: 37px;
line-height: 65px;
font-weight: 500;
color: #242424;
}

.contact__info li a{
  font-family: 'Playfair Display';
font-size: 14px;
line-height: 24px;
font-weight: 400;
color: #797979;
font-family: 'Playfair Bold';
text-decoration: inherit;
color: #e2574c;
}
.contact3__title{
 font-family: Raleway;
font-size: 37px;
line-height: 65px;
font-weight: 500;
color: #242424;
margin-bottom: 40px;
}
.ld{
  margin-top: 30px;
  margin-right: 30px;
}
</style>
