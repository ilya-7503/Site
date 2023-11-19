<template>
  <div class="row narrow-block justify-center q-mt-md q-mb-none">
    <div class="col-12 col-md-8 q-px-xs-md q-px-sm-md q-py-xs-md q-py-md-lg">
      <div class="row narrow-block q-mb-md q-mx-md justify-center items-center">
        <div  class="col-xs-12 col-sm-7">
          <div class=" text-medium" :class="$q.screen.gt.xs?'text-h3':'text-h4 text-center'" >Мебель в стиле лофт</div>
          <div class=" text-weight-regular q-mt-sm q-mb-md" :class="$q.screen.gt.xs?'text-h6':'text-body1 text-center'"> Создаем мебель по вашим эскизам
            и индивидуальным параметрам
          </div>
          <q-img v-if="$q.screen.xs" src="Диван_главная.jpg" class=" q-mb-lg rounded-borders img-size"
                 width="100%" :ratio="6/3"/>
          <div :class="$q.screen.lt.md?'row justify-center':''" >
            <q-btn unelevated class="border-btn text-body1" padding="12px 25px" color="primary" no-caps  label="Рассчитать стоимость"  />
          </div>
        </div>
        <div class="col-xs-10 col-sm-5">
          <q-img v-if="$q.screen.gt.xs" src="Диван_главная.jpg" class="rounded-borders img-size"
                 width="100%"/>
          </div>
      </div>
    </div>
  </div>
  <div class="bg-secondary q-mt-lg">
    <div class="row justify-center narrow-block q-py-xs-lg q-py-sm-xl q-mt-lg q-px-md">
      <div class="col-12 col-md-8 ">
        <div class="row narrow-block q-mx-md  ">
          <div class="col-xs-12 col-sm-6">
            <q-img src="Картинка о нас.jpg" class="rounded-borders "
                   width="100%"  />
          </div>
          <div class="col-xs-12 col-sm " :class="$q.screen.gt.xs?'q-ml-lg':'q-mt-md text-center'" >
            <div class="text-h5 text-weight-medium">О нас</div>
            <div class="text-body1 q-mt-sm">Производственная мастерская основана
              в 2018 году в результате кооперации предприятий
              по изготовлению мебели премиального класса.</div>
            <div class="text-body1 q-mt-sm">Качество нашей мебели - это сочетание стильного дизайна, квалифицированной сборки, технологичного оборудования и контроля на всех этапах производства.
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>


  <div class="row justify-center narrow-block  q-py-xl ">
    <div class="col-12 col-md-8 narrow-block">
      <div class="row justify-center">
        <div class="text-h5  text-weight-medium">Преимущества</div>
      </div>
      <div class="row justify-center  q-mt-md">
        <div class="col-xs-6 col-sm-3 q-pa-md column items-center">
            <q-img src="Производство.svg" width="50px"  />
            <div class="text-body1 text-center q-mt-sm">Собственное <br>
              производство</div>
        </div>
        <div class="col-xs-6 col-sm-3  q-pa-md column items-center">
            <q-img src="Сотрудники.svg" width="50px" />
            <div class="text-body1 text-center q-mt-sm">Опытные<br>
              сотрудники</div>
        </div>
        <div class="col-xs-6 col-sm-3 q-pa-md column items-center">
            <q-img src="Ассортимент.svg" width="50px" />
            <div class="text-body1 text-center q-mt-sm">Широкий <br>
              ассортимент</div>
        </div>
        <div class="col-xs-6 col-sm-3  q-pa-md column items-center">
            <q-img src="Гарантия.svg" width="50px" />
            <div class="text-body1 text-center q-mt-sm">Гарантия <br>
              качества</div>
        </div>
      </div>
    </div>
  </div>

  <div class="row justify-center narrow-block q-px-md ">
    <div class="col-12 col-md-8 narrow-block">
      <div class="row justify-center">
        <div class="text-h5  text-weight-medium q-mb-md">Каталог товаров</div>
      </div>

      <div v-if="$q.screen.gt.xs" class="row justify-center q-mb-md  q-gutter-md ">
        <q-card class="col-xs-12   col-sm border bg-secondary no-shadow">
          <q-card-section>
            <div class="text q-mb-lg">Диваны</div>
            <q-img src="Диван.png" class="rounded-borders"
                   fit="cover"  width="100%" />
          </q-card-section>
        </q-card>
        <q-card class="col-xs-6  col-sm-3 border bg-secondary no-shadow">
          <q-card-section>
            <div class="text q-mb-sm">Кресла</div>
            <q-img src="Кресло.png" class="rounded-borders"
                   fit="cover"  width="100%" />
          </q-card-section>
        </q-card>
        <q-card class=" col-xs-6 col-sm-3 border bg-secondary no-shadow ">
          <q-card-section>
            <div class="text q-mb-sm">Полки</div>
            <div class="row justify-center">
              <div class="col-10">
            <q-img src="Полка.png" class="rounded-borders "
                   fit="cover"  width="100%" />
              </div>
            </div>

          </q-card-section>
        </q-card>
      </div>
      <div v-if="$q.screen.gt.xs" class="row  q-gutter-md">
        <q-card class="col-xs-6 col-sm-3 border bg-secondary no-shadow">
          <q-card-section>
            <div class="text q-mb-sm">Тумбочки</div>
            <div class="row justify-center">
              <div class="col-9">
                <q-img src="Тумбочка.png" class="rounded-borders "
                       fit="cover"  width="100%" />
              </div>
            </div>
          </q-card-section>
        </q-card>
        <q-card class="col-xs-12   col-sm border bg-secondary no-shadow">
          <q-card-section>
            <div class="text q-mb-lg">Подставки под ТВ</div>
            <q-img src="Подставка под ТВ.png" class="rounded-borders"
                   fit="cover"  width="100%" />
          </q-card-section>
        </q-card>
        <q-card class="col-xs-6 col-sm-3 border bg-secondary no-shadow ">
          <q-card-section>
            <div class="text q-mb-sm">Стулья</div>
            <div class="row justify-center">
              <div class="col-6">
                <q-img src="Стул.png" class="rounded-borders "
                       fit="cover"  width="100%" />
              </div>
            </div>
          </q-card-section>
        </q-card>
      </div>

      <div v-if="$q.screen.lt.sm" class="row justify-center q-mb-md q-col-gutter-md">
        <div class="col-xs-12 col-sm">
        <q-card class="border bg-secondary no-shadow">
          <q-card-section>
            <div class="text q-mb-sm">Диваны</div>
            <q-img src="Диван.png" class="rounded-borders"
                   fit="cover"  width="100%" />
          </q-card-section>
        </q-card>
        </div>
        <div class="col-xs col-sm-3">
        <q-card class="col-xs-6  col-sm-3 border bg-secondary no-shadow">
          <q-card-section>
            <div class="text q-mb-sm">Кресла</div>
            <q-img src="Кресло.png" class="rounded-borders"
                   fit="cover"  width="100%" />
          </q-card-section>
        </q-card>
        </div>
        <div class="col-xs col-sm-3">
        <q-card class=" col-xs-6 col-sm-3 border bg-secondary no-shadow ">
          <q-card-section>
            <div class="text q-mb-sm">Полки</div>
            <div class="row justify-center">
              <div class="col-10">
            <q-img src="Полка.png" class="rounded-borders  "
                   fit="cover"  width="100%" />
              </div>
            </div>

          </q-card-section>
        </q-card>
        </div>
      </div>
      <div v-if="$q.screen.lt.sm" class="row justify-center q-col-gutter-md">
        <div class="col-xs-12 col-sm">
          <q-card class=" border bg-secondary no-shadow">
            <q-card-section>
              <div class="text q-mb-sm">Подставки под ТВ</div>
              <q-img src="Подставка под ТВ.png" class="rounded-borders"
                     fit="cover"  width="100%" />
            </q-card-section>
          </q-card>
        </div>
        <div class="col col-sm-3">
          <q-card class=" border bg-secondary no-shadow">
            <q-card-section>
              <div class="text q-mb-sm">Тумбочки</div>
              <div class="row justify-center">
                <div class="col-9">
              <q-img src="Тумбочка.png" class="rounded-borders "
                     fit="cover"  width="100%" />
                </div>
              </div>

            </q-card-section>
          </q-card>
        </div>
        <div class="col col-sm-3 ">
          <q-card class="col-xs col-sm-3 border bg-secondary no-shadow ">
            <q-card-section>
              <div class="text q-mb-sm">Стулья</div>
              <div class="row justify-center">
                <div class="col-6">
                  <q-img src="Стул.png" class="rounded-borders "
                         fit="cover"  width="100%" />
                </div>
              </div>
            </q-card-section>
          </q-card>
        </div>
    </div>
  </div>
  </div>

  <div class="row justify-center  q-py-xl ">
    <div class="col-12 col-md-8 narrow-block">
      <div class="row justify-center">
        <div class="text-h5  text-weight-medium">Схема работы</div>
      </div>
      <div class="row justify-center  q-mt-md">
        <div class="col-xs-6 col-sm-3 q-pa-md column items-center ">
          <q-img src="Консультация.svg" width="50px"  />
          <div class="text-body1 text-center q-mt-sm">Консультация</div>
        </div>
        <div class="col-xs-6 col-sm-3  q-pa-md column items-center">
          <q-img src="Комм. предложение.svg" width="50px" />
          <div class="text-body1 text-center q-mt-sm">Коммерческое <br>
            предложение</div>
        </div>
        <div class="col-xs-6 col-sm-3 q-pa-md column items-center">
          <q-img src="Замер.svg" width="50px" />
          <div class="text-body1 text-center q-mt-sm">Выезд на замер</div>
        </div>
      </div>
      <div class="row justify-center  q-mt-md">
        <div class="col-xs-6 col-sm-3  q-pa-md column items-center">
          <q-img src="Подписание договора.svg" width="50px" />
          <div class="text-body1 text-center q-mt-sm">Подписание <br> договора</div>
        </div>
        <div class="col-xs-6 col-sm-3  q-pa-md column items-center">
          <q-img src="Монтаж.svg" width="50px" />
          <div class="text-body1 text-center q-mt-sm">Монтаж</div>
        </div>
      </div>
    </div>
  </div>

  <div class="bg-secondary">
    <div class="row justify-center narrow-block q-py-xl q-mt-lg q-px-md">
      <div class="col-12 col-md-8 ">
        <div class="row  justify-center narrow-block q-mx-md  ">
          <div class="col-xs-12 col-sm-10 col-md-6 q-ml-none text-left ">
            <div class="text-h5  text-weight-medium" :class="$q.screen.lt.md?'text-center':''">У вас остались вопросы?</div>
            <div class="text-body1 q-mt-sm q-mb-md" :class="$q.screen.lt.md?'text-center':''">Оставьте заявку, и наш менеджер свяжется  с вами, чтобы провести консультацию.</div>
            <q-input v-model="text" outlined  bg-color="white" label="Ваше имя"/>
            <q-input v-model="text1" outlined class="q-mt-md" bg-color="white" label="Ваш телефон"/>
            <div class="row items-center q-mt-md no-wrap q-mb-lg">
              <q-checkbox dense v-model="val" />
              <div class="text-caption q-ml-sm ">Даю согласие на обработку персональных данных</div>
            </div>
            <div :class="$q.screen.lt.md?'row justify-center':''" >
              <q-btn  unelevated class="border-btn text-body1" padding="12px 25px" color="primary" no-caps  label="Оставить заявку"  />

            </div>
          </div>
          <div v-if="$q.screen.gt.sm" class="col q-ml-xl ">
            <q-img src="Кресло и диван.jpg" class="rounded-borders img-size"
                   width="100%" />
          </div>
        </div>
      </div>
    </div>
  </div>

</template>

<script setup>
import {ref} from 'vue'

const val= ref(true)
const text= ref('')
const text1= ref('')
</script>

<style>
.img-size {
  max-width: 570px;
}
.icon-size {

}
</style>
