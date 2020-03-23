<template>
  <q-page class="flex">
    <q-card class="my-card">
      <q-card class="my-card">
      <q-img src="statics/logo-luc.png">
        <div class="text-subtitle2 absolute-top text-center">
          Comércios
        </div>
      </q-img>
    </q-card>
     <q-card-section>
      <q-list bordered>
        <q-item
            clickable
            v-ripple
            v-for="item in comercios"
            :key="item.title"
            v-bind="item">
          <q-item-section avatar>
            <q-icon color="primary" name="shopping_cart" />
          </q-item-section>

            <q-item-section>
              <q-item-label>{{ item.title }}</q-item-label>
              <q-item-label caption lines="1">{{ item.subtitle }}</q-item-label>
              </q-item-section>
        </q-item>
      </q-list>
     </q-card-section>
    </q-card>
  </q-page>
</template>

<script>
export default {
  name: 'PageIndex',
  data () {
    return {
      comercios: [
        {
          title: 'PANIFICADORA LUCRECIA',
          subtitle: 'RUA ANTONIO LEITE, 231, CENTRO',
          img: '',
          link: ''
        },
        {
          title: 'MERCADINHO LUCRECIA',
          subtitle: 'PRACA DA SAUDE, 365, - CENTRO',
          img: '',
          link: ''
        },
        {
          title: 'FARMACIA NOVA LUCRECIA',
          subtitle: 'AVENIDA LAURO MAIA, 433, CENTRO',
          img: '',
          link: ''
        },
        {
          title: 'MADEIREIRA REZENDE',
          subtitle: 'RUA JOAQUIM DIAS, 202, CENTRO',
          img: '',
          link: ''
        },
        {
          title: 'ESPACO LU & JU',
          subtitle: 'AVENIDA GETULIO VARGAS, 393, CENTRO',
          img: '',
          link: ''
        },
        {
          title: 'MERCADINHO ARAUJO',
          subtitle: 'RUA JULIETA DANTAS, 446, CENTRO',
          img: '',
          link: ''
        }
      ]
    }
  }
}
</script>
