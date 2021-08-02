<!-- my-component.vue -->
<template>   
    <p>xxx: {{greeting}}
        <br>
     <van-button type="primary">按钮</van-button>   
        <van-icon name="chat-o" dot size="40"/>
        <br>
        <van-icon name="chat-o" badge="9" size="3rem"  />
        <br>
        <van-icon name="chat-o" badge="99+" color="#ff1111" />
        <br>
        <van-icon name="https://b.yzcdn.cn/vant/icon-demo-1126.png" />
        <br>
        <van-icon name="chat-o" />
        <br>

        
        <van-cell-group inset>
            <van-cell title="单元格1" value="内容1"  size="large"  icon="location-o">
                <template #right-icon>
                    <van-icon name="search" class="search-icon" />
                  </template>

            </van-cell>
            <van-cell title="单元格2" center value="内容2" label="描述信息" is-link arrow-direction="down"  >
                <template #title>
                    <span class="custom-title">单元格3</span>
                    <van-tag type="danger">标签</van-tag>
                  </template>
            </van-cell>

        </van-cell-group>
        
        </p> 
</template> 

<script type='module'>
// import Vant from 'vant' 
// import { Button } from 'vant';
import Button from 'vant/es/button'; 
import 'vant/es/button/style';


import Icon from 'vant/es/icon'; 
import 'vant/es/icon/style';

import Cell from 'vant/es/cell'; 
import 'vant/es/cell/style';


import Cell1 from 'vant/es/cell-group'; 
import 'vant/es/cell-group/style';

export default {
// module.exports={  
    data:function(){  
        return{   
            greeting:'hello'    
        }  
    } ,
    components:{
        // 'van-button': Button,
        [Button.name]:Button,
        [Icon.name]:Icon,
        [Cell.name]:Cell,
        [Cell1.name]:Cell1,
        
    }
} 
</script> 
                          
<style scoped> 
    p{   font-size:2em; }   
</style>