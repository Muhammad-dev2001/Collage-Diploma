<script setup>
$(document).ready(function (){
  var token = 'cc59bf2b1e8c91906145bc2365a62ae67a9fff48';

  $(".address").suggestions({
    token: token,
    type: "ADDRESS",
    onSelect: function(suggestion) {
      console.log(suggestion);
    }
  });

  $(".job").suggestions({
    token: token,
    type: "PARTY",
    onSelect: function(suggestion) {
      console.log(suggestion);
    }
  });

  $(".fio").suggestions({
    token: token,
    type: "NAME",
    onSelect: function(suggestion) {
      console.log(suggestion);
    }
  });
})
//добавил
</script>

<template>
  <!-- Modal -->
  <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <h1 class="modal-title fs-5" id="exampleModalLabel">Закажите свой проект мечты!</h1>
          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
        </div>
        <div class="modal-body">
          <div class="container-fluid justify-content-center">
            <div class="row d-flex justify-content-center">
              <div class="col-12">

                <form method="POST" action="https://formspree.io/f/xlekvjgq">
                  <div class="form-group">
                    <label for="fio" class="mb-2 mt-3 fw-bold">ФИО</label>
                    <input required id="fio" class="form-control fio" type="text" name="name" placeholder="Например, Иванов Иван Иванович" data-reg="^[А-ЯЁ][а-яё]*$">
                  </div>

                  <div class="form-group">
                    <label class="mt-3 fw-bold">Введите номер телефона</label>
                    <input required type="text" class="form-control mt-1" name="phone" placeholder="+7 (999) 99 99 999" data-reg="^((\+7|7|8)+([0-9]){10})$">
                  </div>

                  <div class="form-group">
                    <label class="mt-3 fw-bold">Введите email</label>
                    <input required type="text" class="form-control mt-1" name="email" placeholder="mail@mail.ru" data-reg="^[-\w.]+@([A-z0-9][-A-z0-9]+\.)+[A-z]{2,4}$">
                  </div>

                  <div class="form-group">
                    <label class="mt-3 fw-bold" for="job">Место работы</label>
                    <input required type="text" class="form-control job mt-1" id="job" name="job" placeholder="Например, Оверплан">
                  </div>

                  <div class="form-group">
                    <label class="mt-3 fw-bold" for="date">Дата рождения</label>
                    <input required type="date" class="form-control mt-1" id="date" name="birthday">
                  </div>

                  <div class="form-group">
                    <label class="mt-3 fw-bold" for="address">Адрес прописки</label>
                    <input required type="address" class="form-control address mt-1" id="address" name="address" placeholder="Например, ул. Свободы д. 6">
                  </div>

                  <div class="form-group">
                    <label class="mt-3 fw-bold" for="address">Информация о проекте</label>
                    <textarea required type="message" placeholder="Расскажите о своём проекте!" id="message" name="message" class="form-control  mt-1"></textarea>
                  </div>


                  <div class="col d-flex justify-content-between my-3 mb-5">
                    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Назад</button>
                    <button type="submit" class="btn btn-primary">Отправить</button>
                  </div>

                </form>
              </div><!-- .col-sm-4 -->
            </div> <!-- .row -->

          </div><!-- /.container -->
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
</style>
