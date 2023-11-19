<template>
  <q-layout view="lHh Lpr lFf" style="height: 62px"  >
    <q-header class=" bg-white narrow-block">
      <q-toolbar class="col-md-8 bg-white text-black  justify-center" >
        <q-toolbar-title class="row text-weight-medium q-ma-sm" text-decoration:none>
          <div class="row items-center">
            <a href="#" class="q-mr-sm row items-center text-black">
              <div style="line-height: initial">LOFT</div>
            </a>
            <div v-if="$q.screen.gt.sm" class="q-ml-xs text-center text-body2 row items-center">
              <div class="q-gutter-sm">
                <q-btn  no-caps class="text-weight-regular" flat text-color="black" label="О нас" />
                <q-btn  no-caps class="text-weight-regular" flat text-color="black" label="Преимущества"/>
                <q-btn  no-caps class="text-weight-regular" flat text-color="black" label="Каталог"  />
                <q-btn  no-caps class="text-weight-regular" flat text-color="black" label="Схема работы" />
                <q-btn  no-caps class="text-weight-regular" flat text-color="black" label="Вопросы" />
              </div>
             </div>
          </div>
        </q-toolbar-title>
        <div v-if="$q.screen.gt.sm" class="row items-center q-ma-sm">
          <q-btn class="q-ml-sm border-btn" color="primary" no-caps  outline label="Заказать звонок"  />
          </div>
        <div v-if="$q.screen.lt.md">
          <q-btn flat @click="drawer = !drawer" round dense icon="menu" />
        </div>
      </q-toolbar>
    </q-header>
    <q-drawer v-if="$q.screen.lt.lg"
              v-model="drawer"
              :width="250"
              :breakpoint="1000"
              overlay side="right"
              class="shadow-2"
    >
      <q-scroll-area class="fit">
        <q-list>
          <div class="q-pa-md">
            <div class="row no-wrap ">
            </div>
            <div class="q-mt-sm q-gutter-xs column">
              <q-btn  no-caps class="text-weight-regular" flat text-color="black" label="О нас" />
              <q-btn  no-caps class="text-weight-regular" flat text-color="black" label="Преимущества"/>
              <q-btn  no-caps class="text-weight-regular" flat text-color="black" label="Каталог"  />
              <q-btn  no-caps class="text-weight-regular" flat text-color="black" label="Схема работы" />
              <q-btn  no-caps class="text-weight-regular" flat text-color="black" label="Вопросы" />
              <q-btn class="q-ml-sm border-btn" color="primary" no-caps  outline label="Заказать звонок"  />
            </div>
          </div>
        </q-list>
      </q-scroll-area>
    </q-drawer>
    <q-page-container style="padding-bottom: 0" r>
      <router-view />
    </q-page-container>

    <q-footer  class="q-footer bg-white q-py-md text-black ">
      <div class="row q-toolbar full-width q-pt-sm q-pb-xs-xs q-py-md-sm">
        <div class="col-12 narrow-block q-px-xs-sm q-px-sm-md q-px-xl-none">
          <div class="row items-center justify-center " :class="$q.screen.gt.xs?'q-gutter-md':''" >
            <div class="col-xs-12 col-sm-2 col-md-2 ">
              <div v-if="$q.screen.gt.xs" class="text-weight-medium text-h5">LOFT</div>
              <div v-if="$q.screen.gt.xs" class="row q-mt-xs q-gutter-sm">
                <q-btn flat class="bg-primary border-btn" padding="7px">
                  <q-img src="ВК.png" width="20px" />
                </q-btn>
                <q-btn flat class="bg-primary border-btn" padding="7px">
                  <q-img src="Инст.png" width="20px" />
                </q-btn>
                <q-btn flat class="bg-primary border-btn" padding="7px">
                  <q-img src="Ватсап.png" width="20px" />
                </q-btn>
              </div>
              <div v-if="$q.screen.xs" class="row q-mt-xs q-gutter-sm items-center">
                <div class="col">
                  <div class="text-weight-medium text-h5 ">LOFT</div>
                </div>
                <div class="row justify-end ">
                  <q-btn flat class="bg-primary border-btn" padding="7px">
                    <q-img src="ВК.png" width="20px" />
                  </q-btn>
                  <q-btn flat class="bg-primary q-mx-sm border-btn" padding="7px">
                    <q-img src="Инст.png" width="20px" />
                  </q-btn>
                  <q-btn flat class="bg-primary border-btn" padding="7px">
                    <q-img src="Ватсап.png" width="20px" />
                  </q-btn>
                </div>

              </div>
            </div>
            <div class="col-xs-12 col-sm-5 col-md-3">
              <div class="row q-my-sm " :class="$q.screen.sm?'justify-center':''">
                <div class="column q-gutter-xs">
                  <div class="row q-gutter-xs items-center">
                    <q-btn flat class="bg-primary border-btn" padding="7px">
                      <q-img src="Телефон.png" width="12px" />
                    </q-btn>
                    <div class="text-body1 text-center ">8(919) 883-95-28</div>
                  </div>
                  <div class="row q-gutter-xs items-center">
                    <q-btn flat class="bg-primary border-btn" padding="7px">
                      <q-img src="mail.png" width="12px" />
                    </q-btn>
                    <div class="text-body1 text-center ">loft@gmail.com</div>
                  </div>
                  <div class="row q-gutter-xs items-center no-wrap">
                    <q-btn flat class="bg-primary border-btn" padding="7px">
                      <q-img src="Локация.png" width="12px" />
                    </q-btn>
                    <div class="text-body1 text-center "> г. Москва, ул. Ленина, д. 9</div>
                  </div>
                </div>
              </div>
            </div>

            <div class="col-xs-12 col-sm-3 col-md-3 ">
              <div v-if="$q.screen.sm" class="row justify-center">
                <div  class="column q-gutter-xs row ">
                  <div class="text-body1  ">О нас</div>
                  <div class="text-body1 ">Преимущества</div>
                  <div class="text-body1 ">Каталог</div>
                  <div class="text-body1  ">Схема работы</div>
                  <div class="text-body1  ">Вопросы</div>
                </div>
              </div>

              <div v-if="$q.screen.gt.sm" class="row q-gutter-lg " >
                <div  class="column q-gutter-xs">
                  <div class="text-body1  ">О нас</div>
                  <div class="text-body1 ">Преимущества</div>
                  <div class="text-body1 ">Каталог</div>

                </div>
                <div class="column q-gutter-xs">
                  <div class="text-body1  ">Схема работы</div>
                  <div class="text-body1  ">Вопросы</div>
                </div>
              </div>
              <div v-if="$q.screen.xs" class="row q-gutter-lg q-pt-xs" >
                <div  class="column q-gutter-xs">
                  <div class="text-body1  ">О нас</div>
                  <div class="text-body1 ">Преимущества</div>
                  <div class="text-body1 ">Каталог</div>
                </div>
                <div class="column q-gutter-xs">
                  <div class="text-body1  ">Схема работы</div>
                  <div class="text-body1  ">Вопросы</div>
                </div>
              </div>
            </div>

          </div>
        </div>
      </div>






    </q-footer>

  </q-layout>


</template>

<style lang="sass" scoped>
.my-custom-toggle
  border: 1px solid #51AEE7
</style>

<script>
import { ref } from 'vue'

export default {
  setup () {
    return {
      ssmall: ref(false),
      newtask: ref(false),
      secondModel: ref('one'),
      model: ref(null),
      tab: ref('mails'),
      drawer: ref(false),
      search: ref(''),
      options: [
        'Нет', 'Google', 'Facebook', 'Twitter', 'Apple', 'Oracle'
      ]

    }
  }
}
</script>
