<template>
  <div class="home">
   <Notfier v-show="isModalVisible" @close="closeModal()"/> 

	  
    <button type="button" class="btn" @click="showModal">oi</button>
    
    <carrosell/>
  </div>
 
</template>

<script>
	
// @ is an alias to /src
import Carrosell from '@/components/Carrosell.vue'
import Notfier from '@/components/comps/Notfier.vue'

export default {
  name: 'home',
  components: {
    Carrosell,
      Notfier
  },
    data () {
    return {
      isModalVisible: false,
        
		
    }
  },
    methods:{  
    showModal() {
               
                this.isModalVisible = true;
            },
            closeModal() {
         
                this.isModalVisible = false;
            },}
}
</script>
