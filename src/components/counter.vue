<style scoped>
 .counter {
     display: inline-block;
     -webkit-touch-callout: none;
     -webkit-user-select: none;
     -khtml-user-select: none;
     -moz-user-select: none;
     -ms-user-select: none;
     user-select: none;
     width: 200px;
     height: 200px;
     transition: transform .3s, box-shadow .3s;
     border-radius: 4px;
     box-shadow: 0 0 10px #E2E2E2;
     background-color: #fff;
     margin-top: 20px;
     font-size: 70px;
     text-align: center;
     line-height: 200px;
     border: 1px solid #e2e2e2;
     cursor: pointer;
     &:hover {
	 transform: translateY(-4px);
	 box-shadow: 0 8px 18px rgba(0, 0, 0, 0.2);
     }
 }
</style>

<template>
    <div class="counter" @click="handleClick">
	{{ count }}
    </div>
</template>

<script>
 export default {
     data () {
	 return {
             count: 0
	 }
     },
     ready () {
     },
     methods: {
	 handleClick () {
	     this.count++;
	 }
     }
 }
</script>
