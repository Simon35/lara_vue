<template>
<div class="container-fluid h-100 bg-light text-dark">
  <div class="row justify-content-center align-items-center">
    <h1>Nouveau formulaire avec vue.js</h1>    
  </div>
  <hr/>
  <div class="row justify-content-center align-items-center h-100">
    <div class="col col-sm-6 col-md-6 col-lg-4 col-xl-3">
        <form class="form-group form-inline justify-content-center" @submit.prevent="submitComment">
            <textarea v-model="comment"></textarea><hr>
            <button class="btn dtn-default">Commenter</button>
        </form>
    </div>
  </div>
</div>

</template>

<script>
    export default {
        data(){
            return {
                comment:'',

            }
        },
        methods:{
            submitComment(){
                //console.log('Comment submoitted !!')
                console.log(this.comment);
            }
        }
    }
</script>
