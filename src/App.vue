<template>

<div>
<div>
     <q-tabs v-model="selectedTab">
      <q-tab slot="title" name="tab-1" label="Tab1" icon="message" />
      <q-tab slot="title" name="tab-2" label="tab2" icon="fingerprint"/>
      <q-tab slot="title" name="tab-3" label="Tab3" icon="phone"/>
      </q-tabs>

<q-input v-model="text" />
<q-input v-model="text" stack-label="Stack Label" />
<q-input v-model="text" float-label="Float Label" placeholder="Gigi" />
</div>
 
<div>

  </div>
  </div>
</template>


<script>
import { QTabs, QTab, QBtn } from 'quasar'
export default {
  components: {
    QTabs,
    QTab,
    QBtn
  },
  data () {
    return {
      // initializing for second tab to be selected by default
      selectedTab: 'tab-2'
    }
  },
  methods: {
    selectThirdTab () {
      // we select third tab which has `name` set to 'tab-3'
      this.selectedTab = 'tab-3'
    }
  }
}
</script>

<style>

</style>
