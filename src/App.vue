<template>
  <div id="app">
    <Header></Header>
    <List :userData="userData"></List>
  </div>
</template>

<script>
import Header from './components/Header';
import List from './components/List';
import { MessageBox } from 'mint-ui';
var userData = [
            { "index" : "A", "users" : [
                { "name" : "a1", "tel" : "110" },
                { "name" : "a2", "tel" : "120" },
                { "name" : "a3", "tel" : "130" },
            ] },
            { "index" : "B", "users" : [
                { "name" : "b1", "tel" : "140" },
                { "name" : "b2", "tel" : "150" },
                { "name" : "b2", "tel" : "160" },
                { "name" : "b2", "tel" : "16760" },
                { "name" : "b2", "tel" : "11657650" },
                { "name" : "b2", "tel" : "112340" },
                { "name" : "b2", "tel" : "114530" },
                { "name" : "b2", "tel" : "11453450" },
                { "name" : "b3", "tel" : "114534530" },
            ] },
            { "index" : "C", "users" : [
                { "name" : "c1", "tel" : "45345" },
                { "name" : "c2", "tel" : "45752785" },
                { "name" : "c2", "tel" : "786587" },
                { "name" : "c2", "tel" : "45345" },
                { "name" : "c2", "tel" : "45345" },
                { "name" : "c2", "tel" : "45245" },
                { "name" : "c2", "tel" : "1124130" },
                { "name" : "c2", "tel" : "7865" },
                { "name" : "c2", "tel" : "678362" },
                { "name" : "c2", "tel" : "45345" },
                { "name" : "c2", "tel" : "12321" },
                { "name" : "c3", "tel" : "121212" },
            ] },
            { "index" : "D", "users" : [
                { "name" : "d1", "tel" : "45345" },
                { "name" : "d2", "tel" : "453754412" },
                { "name" : "d3", "tel" : "12312" },
            ] },
            { "index" : "E", "users" : [
                { "name" : "e1", "tel" : "452345" },
                { "name" : "e2", "tel" : "1453245210" },
                { "name" : "e3", "tel" : "5324532" },
            ] },
            { "index" : "F", "users" : [
                { "name" : "f1", "tel" : "4786" },
                { "name" : "f2", "tel" : "3563" },
                { "name" : "f3", "tel" : "12124574" },
            ] },
        ];
export default {
  name: 'App',
  data() {
    return {
      userData : userData
    }
  },
  components: {
    Header,
    List
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
</style>
