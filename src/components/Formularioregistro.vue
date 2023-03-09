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
            motivaciones:"",
            marcas:"",
          };
        },
        methods: {
          submitForm: function () {
            this.formSubmitted = true
          }
        },
      };
    </script>

<template>
    <form>
    <div class="mb-6">
    <label for="name-input" class="block mb-2 text-sm font-medium text-gray-900 dark:text-white">Nombre</label>
    <input type="text" id="name-input" class="block w-full p-4 text-gray-900 border border-gray-300 rounded-lg bg-gray-50 sm:text-md focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500">
</div>
<div class="mb-6">
    <label for="edad-input" class="block mb-2 text-sm font-medium text-gray-900 dark:text-white">Edad</label>
    <input type="text" id="edad-input" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500">
</div>
          <label for="countries" class="block mb-2 text-sm font-medium text-gray-900 dark:text-white">Estado Civil</label>
  <select id="countries" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500">
    <option>Soltero</option>
    <option>Casado</option>
    <option>Divorciado</option>
    <option>Separado</option>
    <option>Union Libre</option>
    <option>Viudo</option>
  </select>
  <div>
    <label for="job-input" class="block mb-2 text-sm font-medium text-gray-900 dark:text-white">trabajo</label>
    <input type="text" id="job-input" class="block w-full p-2 text-gray-900 border border-gray-300 rounded-lg bg-gray-50 sm:text-xs focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500">
</div>
<div>
    <label for="recidencia-input" class="block mb-2 text-sm font-medium text-gray-900 dark:text-white">recidencia</label>
    <input type="text" id="recidencia-input" class="block w-full p-2 text-gray-900 border border-gray-300 rounded-lg bg-gray-50 sm:text-xs focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500">
</div>
<div>
    <label for="appointment-input" class="block mb-2 text-sm font-medium text-gray-900 dark:text-white">Cita</label>
    <input type="text" id="appointment-input" class="block w-full p-2 text-gray-900 border border-gray-300 rounded-lg bg-gray-50 sm:text-xs focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500">
</div>
<div>
    <label for="author quote-input" class="block mb-2 text-sm font-medium text-gray-900 dark:text-white">Cita Autor</label>
    <input type="text" id="author quote-input" class="block w-full p-2 text-gray-900 border border-gray-300 rounded-lg bg-gray-50 sm:text-xs focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500">
</div>
<div>
    <label for="bio-input" class="block mb-2 text-sm font-medium text-gray-900 dark:text-white">Bio</label>
    <input type="text" id="bio-input" class="block w-full p-2 text-gray-900 border border-gray-300 rounded-lg bg-gray-50 sm:text-xs focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500">
</div>
<button lass="btn btn-default" @enviar="enviar" type="submit" class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">Registra tu persona</button>
</form>
    </template>
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
  