<template>
    <div id="lnput">
        <el-input
            size="mini"
            @change="valideMsg" 
            placeholder="请输入内容"
            v-model="input_value"
            clearable>
        </el-input>
    </div>
</template>
<script>
export default {
    data(){
        return {
           input_value: null,
        }
    },

    methods:{
       valideMsg(){
           if(this.input_value == 'B'){
               alert("名字冲突");
           }
       }
    }
}
</script>
<style scoped>

</style>