<template>
  <div class="home">
    <div class="header">
      <h2 class="title">Bienvenido a <b>Pasteleria Boris</b></h2>
      <div class="input">
        <input type="text" placeholder="busca lo que deceas" />
        <div class="icon-search">
          <i class="bx bx-search-alt-2"></i>
        </div>
      </div>
      <div class="combo-header">
        <div class="text">
          <h3 class="conejitos">
            CREPE CAKE CONEJITOS.
            <p>
              Crepas de vainilla, relleno de crema de chocolate con leche,
              decorado con conejo de chocolate.
            </p>
          </h3>
        </div>
        <div class="imagen">
          <img
            src="https://file.adomicil.io/esperanza.tr3sco.net/_files/images/product/imagen-8-0683851078005438.png"
            alt=""
            class="img"
          />
        </div>
      </div>
    </div>
  </div>
  <div class="scroll-menu">
    <div class="scroll-content">
      <div :key="index" class="avatar" v-for="(item, index) in 10">
        <i class="bx bx-cake bx-sm"></i>
      </div>
    </div>
  </div>
  <h2 class="pasteles">Top Pasteles</h2>

  <div class="scroll-menu">
    <div class="scroll-content">
    <div :key="index" v-for="(item,index) in 10"  class="top-pasteles">
      <div class="top-pasteles-img">
        <img  src="https://file.adomicil.io/esperanza.tr3sco.net/_files/images/product/thumb3-0503600571539067.jpg" alt="" />
      </div>
      <div class="top-pasteles-titulo">pastel de coco</div>
      <div class="top-pasteles-precio">
        <h4>$399.99</h4>
      </div>
      <div class="top-pasteles-precio-accion">
        <i class="bx bx-plus"></i>
      </div>
    </div>
  </div>
  </div>

   

</template>

<style >
.pasteles {
  padding-top: 20px;
  font-weight: 400;
  color: #000;
  font-style: normal;
  font-family: Arial, Helvetica, sans-serif;
}
.text {
  width: 50%;
}
.imagen {
  width: 50%;
  object-fit: cover;
}
.img {
  width: 80%;
  display: flex;
}
.conejitos {
  font-weight: 300px;
}
p {
  font-weight: 300;
}
.home {
  margin: 20px;
  text-align: initial;
  font-family: "Fredoka One", cursive;
  font-family: "Oswald", sans-serif;
  color: rgb(0, 0, 0);
}
.header .input {
  width: 100%;
  display: flex;
  position: relative;
  align-items: center;
  margin-top: 15px;
}

.header .icon-search {
  position: absolute;
  margin-left: 10px;
}

.header .combo-header {
  background-color: rgb(24, 122, 29);
  color: #fff;
  padding: 10px;
  border-radius: 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-radius: 20px;
  margin-top: 20px;
}

input {
  width: 100%;
  background-color: rgba(46, 44, 44, 0.116);
  border: 0px;
  outline: none;
  padding: 10px;
  padding-left: 30px;
  border-radius: 10px;
}

.title {
  font-weight: 400;
  text-align: initial;
}

.scroll-menu {
  width: 100%;
}
.scroll-content {
  display: flex;
  overflow-y: auto;
}

.avatar {
  background-color: rgba(58, 56, 56, 0.11);
  padding: 10px;
  border-radius: 10px;
  margin: 10px;
  height: 30px;
}

.avatar i {
  color: rgb(226, 144, 21);
}


.top-pasteles {
  min-width: 150px;
  background-color: rgba(43, 43, 43, 0.103);
  position:relative;
  border-radius: 20px;
  padding: 10px;
   margin: 10px;

}

.top-pasteles-img{
   display: flex;
}

.top-pasteles-precio-accion i {
  padding: 10px;
  border-radius: 50px;
  background-color: rgb(4, 112, 1);
  color: #fff;
  position: absolute;
  right: 0;
  bottom: 0;
  margin: 10px;
}
.top-pasteles-titulo{
  color: rgb(0, 0, 0, 100);
  text-align: initial;
  margin: 10px;
}

.top-pasteles-precio{
  color: rgb(219, 110, 8);
  text-align: initial;
  margin: 10px;

}
.top-pasteles-img img{
  width: 100px;

}

</style>
