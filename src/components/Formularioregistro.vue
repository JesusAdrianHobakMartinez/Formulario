<template>
    <div class="about">
    </div>
      <div>
        <form @submit.prevent="submitForm" v-if="!formSubmitted">
          <span>Nombre</span><br>
          <input 
            v-model="name"
            type="text"
            placeholder="Nombre" 
          /><br>
          <span>Apellidos</span><br>
          <input 
            v-model="apellido"
            type="text"
            placeholder="apellidos" 
          /><br>
          <span>Motivacion</span><br>
          <input 
            v-model="email"
            type="motivasión"
            placeholder="Pon tu motivasión" 
          /><br>
          <span>Sexo</span><br>
          <input 
            type="radio" 
            v-model="sexo" 
            value="Male" 
          />
          <label>Masculino</label>
          <input 
            type="radio" 
            v-model="gender" 
            value="Female" 
          />
          <label>Femenino</label><br>
          <input 
            class="submit" 
            type="submit" 
            value="Submit"
          >
          <label for="countries" class="block mb-2 text-sm font-medium text-gray-900 dark:text-white">Estado Civil</label>
  <select id="countries" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500">
    <option>Soltero</option>
    <option>Casado</option>
    <option>Divorciado</option>
    <option>Separado</option>
    <option>Union Libre</option>
    <option>Viudo</option>
  </select>
        </form>
        <div v-if="formSubmitted">
          <h3>Form Submitted</h3>
          <p>Nombre: {{ name }}</p>
          <p>Apellidos: {{ apellidos }}</p>
          <p>Motivasion: {{ motivasion }}</p>
          <p>Sexo: {{ sexo }}</p>
          <small>Click on run to launch the app again.</small>
        </div>
      </div>
    </template>
    <script>
      export default {
        data() {
          return {
            name: "",
            edad:"",
            estadocivil:"",
            trabajo:"",
            recidencia:"",
            cita:"",
            citaautor:"",
            bio:"",
            personalidad1:"",
            personalidad2:"",
            personalidad3:"",
            personalidad4:"",
            objetivos:"",
            frustaciones:"",
            motivaciones:"value",
            sexo: "",
            formSubmitted: false
          };
        },
        methods: {
          submitForm: function () {
            this.formSubmitted = true
          }
        },
      };
    </script>
    <style>
      form {
        padding: 10px;
        border: 2px solid black;
        border-radius: 5px;
      }
    
      input {
        padding: 3px 4px;
        margin: 4px;
      }
    
      span {
        font-size: 18px;
        margin: 4px;
        font-weight: 500;
      }
    
      .submit {
        font-size: 15px;
        color: #fff;
        background: #222;
        padding: 6px 12px;
        border: none;
        margin-top: 8px;
        cursor: pointer;
        border-radius: 5px;
      }
    
    </style>
  