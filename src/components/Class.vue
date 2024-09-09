<template>

    <div class="border w-[550px] rounded p-5 my-5 mx-auto " >
      <h2 class="font-bold text-3xl text-center " > V-model</h2>
    
      <div class="flex justify-between items-center mt-5">
        <input type="text" class="border p-2 w-[300px] rounded" placeholder="Enter your name" v-model="name" />
        <button class="bg-blue-500 text-white px-3 py-2 rounded" @click="addName" >Add Name</button>
      </div>
    
    
      <div class="mt-5">
        <ul>
          <li  class="border p-2 my-2 rounded" > Name: <strong> {{names}} </strong> </li>
        </ul>
      </div>
    
      <hr>
    
      <div>
        <h2 class="font-bold text-2xl text-center"> Increase & Decrease </h2>
    
        <div class="flex justify-between items-center mt-5">
          <button class="bg-blue-500 text-white px-3 py-2 rounded" @click="decrease" >-</button>
          <input type="text" class="border p-2 w-[100px] rounded text-center" v-model="number"   />
          <button class="bg-blue-500 text-white px-3 py-2 rounded" @click="increase" >+</button>
        </div>
      </div>
    
      <hr> 
    
      <!-- v-for -->
      <div class="my-3 ">
        <h2 class="font-bold text-2xl text-center"> V-for  </h2>
    
        <div v-for="arrays in array" :key="arrays.id" class="p-1 ">
          <p v-if="arrays.status" class="bg-[#1b9736] text-white p-1 rounded "  > {{arrays.name}} {{ array.status }} </p>
          <p v-else class="bg-[#eb2d2d] text-white p-1 rounded "  > {{arrays.name}} {{ array.status }} </p>
    
        </div>
    
        <ul>
          <li v-for="item in array" :key="item.id" class="border p-2 my-2 rounded" >
            <strong> {{item.name}} </strong> 
            <span v-if="item.status" class="text-green-500" >  Active </span>
            <span v-else class="text-red-500" > Inactive </span>
          </li>
        </ul>
        
      </div>
    </div>
    
    </template>
    
    <script>
    
    export default{
      data(){
        return{
          name:'',
          names:'',
          number:0,
    
          array:[
            {id:1, name:'John', status:true },
            {id:2, name:'Doe', status:false },
            {id:3, name:'Smith', status:true },
            {id:4, name:'Alex', status:false },
            {id:5, name:'Jenny', status:true },
            {id:6, name:'Marry', status:false },
            {id:7, name:'Doe', status:true },
            {id:8, name:'Smith', status:false },
            {id:9, name:'Alex', status:true },
            {id:10, name:'Jenny', status:false },
          ]
        }
      },
    
      methods:{
        addName(){
          this.names=this.name
          this.name=''
          // alert(this.name)
        },
    
        increase(){
          this.number ++
        },
        decrease(){
          if (this.number>0){
            this.number --
          }
        },
      }
    
    
    }
    
    </script>