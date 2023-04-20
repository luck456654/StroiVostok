<template>
  <div>
    <div class="container">
      <h2 class="title">Цены кровельного покрытия</h2>
      <div class="flex">
        <table class="table">
          <tbody>
            <tr class="table__head">
              <th>
                Наименование
              </th>
              <th>цена на кровельное покрытие с утеплителем</th>
              <th>цена на кровельное покрытие без утеплителя</th>
              
            </tr>
            <tr>
             <td>Монтаж кровли из металлочерепицы</td> 
             <td>1500 руб./м</td>
             <td>1100 руб./м</td>
            </tr>
            <tr>
             <td>Монтаж мягкой кровли</td> 
             <td>0т 1950 руб./м</td>
             <td>1600 руб./м</td>
            </tr>
             <td>Монтаж битумной черепицы</td> 
             <td></td>
             <td></td>
            </tr>
            <tr class="bggray">
             <td>Монтаж керамической черепицы</td> 
             <td></td>
             <td ></td>
            </tr>
            <tr>
             <td>Монтаж кровли из профнастила / профлиста</td> 
             <td>1250 руб./м</td>
             <td>1100 руб./м</td>
            </tr>
            <tr class="bggray">
             <td></td> 
             <td></td>
             <td ></td>
            </tr>
            <tr>
             <td>Монтаж кровли из сэндвич панелей</td> 
             <td></td>
             <td></td>
            </tr>
            <tr>
             <td>Монтаж мембранной кровли</td> 
             <td>от 1500 руб./м</td>
             <td></td>
            </tr>
            <tr class="bggray">
             <td>Монтаж кровли из шифера</td> 
             <td></td>
             <td ></td>
            </tr>
            <tr>
             <td>Монтаж медной кровли</td> 
             <td></td>
             <td></td>
            </tr>
            <tr class="bggray">
             <td>Монтаж мембранной кровли</td> 
             <td></td>
             <td ></td>
            </tr>
            <tr>
             <td>Монтаж наплавляемой кровли</td> 
             <td>0т 400 руб./м</td>
             <td></td>
            </tr>
            <tr>
             <td>Монтаж мягкой кровли</td> 
             <td>0т 1950 руб./м</td>
             <td>1600 руб./м</td>
            </tr>
            <tr class="bggray">
             <td>Монтаж натуральной черепицы</td> 
             <td></td>
             <td ></td>
            </tr>
            <tr>
             <td>Монтаж ондулина на кровлю</td> 
             <td></td>
             <td></td>
            </tr>
            <tr class="bggray">
             <td>Монтаж сланцевой кровли</td> 
             <td></td>
             <td ></td>
            </tr>
            <tr>
             <td>Монтаж фальцевой кровли</td> 
             <td></td>
             <td></td>
            </tr>
            <tr class="bggray">
             <td>Укладка рубероида на крышу</td> 
             <td></td>
             <td ></td>
            </tr>
            <tr>
             <td>Установка композитной черепицы</td> 
             <td></td>
             <td></td>
            </tr>
           </tbody>
        </table>
      </div>
      <div class="tablewrapp">
        <div v-for="(item, index) in items" :key="index" class="mtable">
          <div class="mtable__tr">
            <div class="mtable__title">Название</div>
            <div class="mtable__desck">{{ item.name }}</div>
          </div>
          <div class="mtable__tr">
            <div class="mtable__title">цена на кровельное покрытие с утеплителем</div>
            <div class="mtable__desck">{{ item.priceins }}</div>
          </div>
          <div class="mtable__tr bordernone">
            <div class="mtable__title">цена на кровельное покрытие без утеплителя</div>
            <div class="mtable__desck">{{ item.pricenoins }}</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "TableKrovlya",
  data() {
    return {
      items: [
      { name: "Монтаж кровли из металлочерепицы", priceins:"1400 руб./метр",pricenoins:"1100 руб./метр" },
      { name: "Монтаж мягкой кровли", priceins:"1950 руб./метр",pricenoins:"1600 руб./метр" },
      { name: "Монтаж битумной черепицы", priceins:"",pricenoins:"" },
      { name: "Монтаж керамической черепицы", priceins:"",pricenoins:"" },
      { name: "Монтаж кровли из профнастила / профлиста", priceins:"1250 руб./метр",pricenoins:"1100 руб./метр" },
      { name: "Монтаж кровли из сэндвич панелей", priceins:"",pricenoins:"" },
      { name: "Монтаж кровли из шифера", priceins:"",pricenoins:"" },
      { name: "Монтаж медной кровли", priceins:"",pricenoins:"" },
      { name: "Монтаж мембранной кровли", priceins:"от 1500 руб./метр",pricenoins:"" },
      { name: "Монтаж наплавляемой кровли", priceins:" от 400 руб./метр",pricenoins:"" },
      { name: "Монтаж натуральной черепицы", priceins:"",pricenoins:"" },
      { name: "Монтаж ондулина на кровлю", priceins:"",pricenoins:"" },
      { name: "Монтаж сланцевой кровли", priceins:"",pricenoins:"" },
      { name: "Монтаж фальцевой кровли", priceins:"",pricenoins:"" },
      { name: "Укладка рубероида на крышу", priceins:"",pricenoins:"" },
      { name: "Установка композитной черепицы", priceins:"",pricenoins:"" },      
      ],
    };
  },
};
</script>
<style scoped>
@font-face {
  font-family: "Geometria";
  font-style: normal;
  font-weight: 400;
  src: url("./fonts/geometria/Geometria-Medium.woff2") format("woff2");
}
.flex {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
.bordernone{
  border-bottom: none!important;
}
.container {
  display: flex;
    flex-direction: column;
    width: 100vw;
    align-items: center;
}
.title {
  text-align: center;
}
.table {
  border-collapse: collapse;
  font-size: 0.83vw;
  font-family: "Geometria";
  margin-bottom: 4vw;
}
.table__head {
  background-color: #ff3f3f;
  color: white;
}
td {
  padding: 0.75rem;
}
.bggray {
  background-color: #f2f2f2;
}
th {
  padding: 0.5vw;
}
.mtable {
  display: none;
}

@media (max-width: 767px) {
  .table {
    display: none;
  }
  .mtable {
    display: block;
    border: 1px solid#ccc;
    width: 70.7vw;
    margin-bottom: 2vw;
  }
  .mtable__title,
  .mtable__desck {
    font-family: "Geometria";
    font-size: 1.83vw;
    text-transform: uppercase;
  }
  .mtable__tr {
    display: flex;
    padding: 1.5vw;
    border-bottom: 1px dotted #ccc;
    margin-left: 1vw;
    margin-right: 1vw;
    font-family: sans-serif;
  }
  .mtable__title {
    width: 25vw;
    font-weight: bold;
  }
  .tablewrapp {
    overflow-y: scroll;
    flex-wrap: wrap;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    height: 68vw;
    padding: 5vw;
    margin-left: 10vw;
  }
  .container{
    padding-left: 0;
  }
  .brdnone{
    border: none;
  }
 }
 @media (max-width: 500px) {
  .tablewrapp{
    flex-direction: row;
    overflow-y: scroll;
    justify-content: space-between;
    margin-left: 12vw;
    height: 100vw;
  }
  .mtable{
    width: 66.7vw;
  }
  .mtable__desck,.mtable__title {
    font-family: "Geometria";
    font-size: 2.83vw;
    text-transform: uppercase;
    max-width: 29vw;
  }
  .mtable__title {
    width: 29vw;
  }
 }
</style>