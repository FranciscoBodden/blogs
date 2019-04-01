<template>
  <div class="hello">
    <div class="navbar-fixed">
      <nav class="blue">
        <div class="container">
          <div class="nav-wrapper">
            <a href="#!" class="brand-logo">Viajes RD</a>
            <a href="#" data-target="mobile-demo" class="sidenav-trigger">
              <i class="material-icons">menu</i>
            </a>
            <ul class="right hide-on-med-and-down">
              <li>
                <a href="#inicio">Inicio</a>
              </li>
              <li>
                <a href="#Posts">Posts</a>
              </li>
              <li>
                <a href="#gallery">Galeria</a>
              </li>
              <li>
                <a href="#contact">Contact</a>
              </li>
            </ul>
          </div>
        </div>
      </nav>
    </div>
    <ul class="sidenav" id="mobile-demo">
      <li>
        <a href="#inicio">Inicio</a>
      </li>
      <li>
        <a href="#Posts">Posts</a>
      </li>
      <li>
        <a href="#gallery">Galeria</a>
      </li>
      <li>
        <a href="#contact">Contact</a>
      </li>
    </ul>

    <!-- Section: Portada -->
    <section id="inicio" class="slider">
      <img src="https://image.ibb.co/hbEMux/resort1.jpg" width="100%" height="100%" alt>
    </section>

    <!-- Section: Icon Boxes -->
    <section class="section section-icons grey lighten-4 center">
      <div class="container">
        <div class="row">
          <div class="col s12 m4">
            <div class="card-panel">
              <img
                class="circle responsive-img"
                src="https://3j0grh44ocny4a6kcn288izx-wpengine.netdna-ssl.com/wp-content/uploads/2017/09/iberostar-950x530.jpg"
              >
              <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quidem, velit.</p>
            </div>
          </div>
          <div class="col s12 m4">
            <div class="card-panel">
              <img
                class="circle responsive-img"
                src="https://www.volunteerforever.com/uploads/editor_uploads/volunteer-in-caribbean-dominican-republic(1).jpg"
              >
              <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quidem, velit.</p>
            </div>
          </div>
          <div class="col s12 m4">
            <div class="card-panel">
              <img
                class="circle responsive-img"
                src="http://s9416.pcdn.co/wp-content/uploads/2015/12/punta-cana-dominican-republic-davidsbeenhere-jpg.jpg"
              >
              <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quidem, velit.</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Section: Posts -->
    <section id="Posts" class="section section-Posts scrollspy">
      <div class="container">
        <div class="row">
          <h4 class="center">
            <span class="teal-text">Posts</span>
          </h4>
          <div class="col s12 m4">
            <div class="card">
              <div class="card-image">
                <img
                  src="http://blog.cataloniahotels.com/es/blog/wp-content/uploads/2017/09/zona-colonial-santo-domingo-876x490.jpg"
                  alt
                >
                <span class="card-title">Zona colonial, Santo Domingo</span>
              </div>
              <div class="card-content">
                <p>
                  Lorem ipsum dolor, sit amet consectetur adipisicing elit. Voluptas aliquid fugiat corporis laudantium, architecto
                  delectus?
                </p>
                <hr>
                <input placeholder="Comentario" type="text" v-model="coment1">
                <input @click=" agregarcoment4" type="submit" value="Comentar" class="btn">
                <ul>
                  <li v-for="comentss of coments2" :key="comentss">{{comentss.comt}}</li>
                </ul>
              </div>
            </div>
          </div>
          <div class="col s12 m4">
            <div class="card">
              <div class="card-image">
                <img
                  src="https://www.planetware.com/photos-large/DOM/dominican-republic-puerto-plata-forte-san-felipe.jpg"
                  alt
                >
                <span class="card-title">Puerto Plata</span>
              </div>
              <div class="card-content">
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
                <hr>
                <input placeholder="Comentario" type="text" v-model="coment2">
                <input @click=" agregarcoment3" type="submit" value="Comentar" class="btn">
                <ul>
                  <li v-for="comentss of coments3" :key="comentss">{{comentss.comt}}</li>
                </ul>
              </div>
            </div>
          </div>
          <div class="col s12 m4">
            <div class="card">
              <div class="card-image">
                <img src="http://greatruns.com/wp-content/uploads/2018/11/Samana%CC%81_9.jpg" alt>
                <span class="card-title">Samana</span>
              </div>
              <div class="card-content">
                <p>
                  Lorem ipsum dolor, sit amet consectetur adipisicing elit. Voluptas aliquid fugiat corporis laudantium, architecto
                  delectus?
                </p>
                <hr>
                <input placeholder="Comentario" type="text" v-model="coment3">
                <input @click=" agregarcoment2" type="submit" value="Comentar" class="btn">
                <ul>
                  <li v-for="comentss of coments4" :key="comentss">{{comentss.comt}}</li>
                </ul>
              </div>
            </div>
          </div>
          <div class="col s12 m4">
            <div class="card">
              <div class="card-image">
                <img
                  src="http://2.bp.blogspot.com/-T8hJAhWUMhE/Ulr4YplUctI/AAAAAAAAAyw/tolp8-A_M4E/s1600/SAM_1784.JPG"
                  alt
                >
                <span class="card-title">Pico Duarte</span>
              </div>
              <div class="card-content">
                <p>
                  Lorem ipsum dolor, sit amet consectetur adipisicing elit. Voluptas aliquid fugiat corporis laudantium, architecto
                  delectus?
                </p>s
                <hr>
                <input placeholder="Comentario" type="text" v-model="newcoment">
                <input @click="agregarcoment" type="submit" value="Comentar" class="btn">
                <ul>
                  <li v-for="comentss of coments" :key="comentss">{{comentss.comt}}</li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      coments: [{ comt: "Excelente" }, { comt: "nice" }, { comt: "cool" }],
      coments2: [{ comt: "" }],
      coments3: [{ comt: "" }],
      coments4: [{ comt: "" }],
      newcoment: "",
      coment3: "",
      coment2: "",
      coment1: "",
      hey: "holaa"
    };
  },
  methods: {
    agregarcoment() {
      this.coments.push({
        comt: this.newcoment
      });
      this.newcoment = "";
    },
    agregarcoment2() {
      this.coments4.push({
        comt: this.coment3
      });
      this.coment3 = "";
    },
    agregarcoment3() {
      this.coments3.push({
        comt: this.coment2
      });
      this.coment2 = "";
    },
    agregarcoment4() {
      this.coments2.push({
        comt: this.coment1
      });
      this.coment1 = "";
    }
  }
};
</script>
<style scoped>
</style>
