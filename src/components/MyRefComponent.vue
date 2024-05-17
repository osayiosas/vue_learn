<script setup>
import { reactive, ref } from "vue";

let count = ref(0);

let username = ref("");

let userslist = ref(["osayi", "james", "john"]);

let userinfo = ref({
  name: "Ola",
  email: "ola@gmail.com",
  age: 30,
  location: ["Nigeria", "Lagos"],
  isMarried: true,
});

let friends = reactive([
  ref("Osayi"),
  ref("James"),
  ref("John"),
  ref("Idiaghe"),
]);
</script>

<template>
  <h1>Count: {{ count }}</h1>
  <button @click="count++">++</button>
  <button @click="count--">--</button>

  <h1>Name: {{ username }}</h1>

  <button @click="username = 'osayi'">Add Name</button>

  <h1>Users: {{ userslist }}</h1>
  <button @click="userslist.push('idiaghe', 'ernest')">add users</button>

  <h1>Name: {{ userinfo.name }}</h1>
  <h1>Email: {{ userinfo.email }}</h1>
  <h1>Age: {{ userinfo.age }}</h1>
  <h1>Location: {{ userinfo.location }}</h1>
  <h1>isMarried: {{ userinfo.isMarried }}</h1>

  <button @click="userinfo.name = 'james'">Change Name</button>
  <button @click="userinfo.email = 'idgaheosaigbovo@gmail.com'">
    Change Email
  </button>
  <button @click="userinfo.age = 40">Change Age</button>
  <button @click="userinfo.location = ['Nigeria', 'Edo']">
    Change Location
  </button>
  <button @click="userinfo.isMarried = false">Change isMarried</button>

  <h1>0: {{ friends[0] }}</h1>
  <h1>1: {{ friends[1] }}</h1>
  <h1>2: {{ friends[2] }}</h1>
  <h1>3: {{ friends[3] }}</h1>

  <button @click="friends[0] = 'Hi'">shake hands</button>
  <button @click="friends[1] = 'hello'">shake hands</button>
  <button @click="friends[2] = 'whatsup'">shake hands</button>
  <button @click="friends[3] = 'bye'">shake hands</button>
</template>
