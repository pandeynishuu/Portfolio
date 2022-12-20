<template>
  <template-view>
 <main>
  <section>
    <div class="body">
      <!-- intro section -->
      <div style="padding-top:90px; ">
        <div class="container">
          <div class="row" >
            <div class="col-md-6">
             <div style="padding-top:90px; ">
              <div style="color: #81b622;padding-left:40px;">
                <h5>Hi , my name is</h5>
              </div>
              <div style="color: white; font-weight:bold; font-size:55px; padding-left:40px;">
                <p>Nisha Pandey.</p>
              </div>
              <div style="color: grey;font-weight:bold; font-size:40px;padding-left:40px;">
                <h1>I'm a Front-End Developer</h1>
              </div>
            
              <div style="margin: 10px 10px 10px 10px; padding-left:40px;">
                <button
                  type="button"
                  class="btn"
                  style="
                    background-color: #071125; 
                    color: #81b622;
                    border: 1px solid #81b622;
                    padding: 10px 15px 10px 15px;
                  "
                >
                 Contact Me
                </button>
               
              </div>
             </div>
            </div>
            <div class="col-md-6">
              <img src="../assets/me-removebg-preview.png" alt="" style="width:70%;">
            </div>
          </div>
        </div>
      </div>
      <about-view  id="about"/>   
      </div>
   </section>
 </main>
  </template-view>
</template>

<script>
import TemplateView from "@/views/TemplateView";
import AboutView from '@/views/AboutView'
// @ is an alias to /src

export default {
  name: "HomeView",
  components: {
    TemplateView,
    AboutView
  },
};
</script>

<style scoped>


</style>
