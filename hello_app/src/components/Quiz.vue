<template>
    <div class="alert alert-primary">
        <h2>クイズ作る</h2>
        <p>{{ quiz_text }}</p>
    </div>
</template>
<script>

//お決まりでつけよう
export default{
    name:'Quiz',
    props:{
        quiz_text:String
    }
}
</script>