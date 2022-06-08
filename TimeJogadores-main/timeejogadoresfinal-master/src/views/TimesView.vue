<script>
export default {
 data(){
   return {
     times: [
       {id: 1, name:"Time 1"},
       {id: 2, name:"Time 2"},
       {id: 3, name:"Time 3"},
       {id: 4, name:"Time 4"},
     ],
    };
   },
 };
</script>


<template>
  <div class="container"> 
    <div class="title"> 
      <h2>Gerenciamento de Times </h2>
    </div>
    <div class="form-input">
      <input type="text" />
      <button>Salvar</button>
   </div>
   <div class="list-items">
    <table>
        <thead>
          <tr>
            <th>ID</th>
            <th>Nome</th>
            <th>Idade</th>
            <th>Times</th>
            <th>Ações</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="time in times " :key="time.id">
          <td>{{ time.id }}</td>
          <td>{{ time.name }}</td>
          <td>???</td>
          </tr>
        </tbody>

      </table>
    </div>
  </div>
</template>


