<template>
    <mt-index-list>
        <mt-index-section v-for="(item,index) in userData" :key="index" :index="item.index">
            <mt-cell @click.native="telAlert(user.tel)" v-for="(user,index) in item.users" :key="index" :title="user.name"></mt-cell>
        </mt-index-section>
    </mt-index-list>
</template>

<script>
import { MessageBox } from 'mint-ui';

 export default {
    name: 'List',
    props : {
        'userData' : {
            type : Array,
            default : function(){
                return [];
            }
        }
    },
      methods : {
      telAlert : function(tel){
        MessageBox({
            title: '呼叫',
            message: tel,
            showCancelButton: true
        });
      }
  }
    
    
 }
</script>

<style scoped>

 
</style>
