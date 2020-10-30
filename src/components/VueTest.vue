<template>
    <div id="dynamicList">
        <h1>{{listName}}</h1>
        <div id="list" style="border-style: solid; border-width: 1px; border-color: black; height: 400px; width: 400px; overflow: auto; margin-bottom: 5px;">
            <ul>
                <li v-for="item in currentList" v-bind:key="item">{{item}}</li>    
            </ul>
        </div>
        <input type="text" v-model="this.currentText" style="width:400px">
        <br/>
        <button v-on:click="addToList" style="margin-right:15px">Add</button>
        <button v-on:click="clearList">Clear</button>
    </div>
</template>

<script>
export default {
  el: "#dynamicList",
  name: "DynamicList",
  data()
  {
      return {
          currentText: "",
          currentList: 
          [

          ]
      }
  },
  props: {
    listName: String
  },
  methods: {
    addToList()
    {
        this.currentList.push(this.currentText);
    },
    clearList()
    {
        this.currentList = [];
    }
  }
};
</script>