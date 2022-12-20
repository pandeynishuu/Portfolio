<template>
  <div>
    <nav class="navbar navbar-expand-lg">
      <div class="container-fluid">
        <a class="navbar-brand" href="#thichindaina ta hau"
          ><img
            src="../assets/nisha_logo-removebg-preview.png"
            alt="Max-width 100%"
            style="height: 45px"
        /></a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNavDropdown"
          aria-controls="navbarNavDropdown"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNavDropdown">
          <ul class="navbar-nav ms-auto">
            <li class="nav-item"  style="padding: 0px 15px 0px 15px">
              <a
                class="nav-link active"
                aria-current="page"
                href="#about"
                >1.About</a
              >
            </li>
            <li class="nav-item" style=" padding: 0px 15px 0px 15px">
              <a
                class="nav-link active"
                aria-current="page"
                href="#exp"
               
                >2.Experience</a
              >
            </li>
            <li class="nav-item" style="padding: 0px 15px 0px 15px">
              <a
                class="nav-link active"
                aria-current="page"
                href="#work"
                >3.Work</a
              >
            </li>
            <li class="nav-item" style="padding: 0px 15px 0px 15px">
              <a
                class="nav-link active"
                aria-current="page"
                href="#contact">4.Contact</a
              >
            </li>
           <a href="" @click.prevent="$router.push({ name: 'resume' })">
            <button
            type="button"
            class="btn"
            style="
              background-color: #071125;
              color: #81b622;
              border: 1px solid #81b622;
              padding: 5px 15px 5px 15px;
            "
          >
            Resume
          </button>
           </a>
            
          </ul>
        </div>
      </div>
    </nav>

    <div class="side_element">
      <ul class="element_menu">
        <li>
          <a href="https://github.com/pandeynishuu" target="_blank"><i class="fa-brands fa-github icon"></i></a>
        </li>
        <li>
          <a href="" target="_blank"><i class="fa-brands fa-instagram"></i></a>
        </li>
        <li>
          <a href="https://twitter.com/Nisha789Pandey" target="_blank"><i class="fa-brands fa-twitter"></i></a>
        </li>
        <li>
          <a href="https://www.linkedin.com/in/nisha-pandey-2960b9218/" target="_blank"><i class="fa-brands fa-linkedin"></i></a>
        </li>
      </ul>
    </div>

    <div class="right_element">
      <div>
        <a href="" >np0091459@gmail.com</a>
      </div>
    </div>
  </div>
  
</template>

<script>
export default {
  name: "NavbarComponent",
};
</script>

<style scoped>
.navbar {
  background-color: #071125;
  font-family: "SF Mono", "Fira Code", "Fira Mono", "Roboto Mono", monospace;
  font-weight: bold;
}
a{
  color: grey;
}
a:hover {
  color: #81b622;
}
.side_element { 
  width: 40px; 
  position: fixed; 
  bottom: 0px; 
  left: 40px; 
  right: auto; 
  z-index: 10; 
  color: white ; 
}
.right_element { 
  width: 40px; 
  position: fixed; 
  bottom: 0px; 
  left: auto; 
  right: 40px; 
  z-index: 10; 
  color: white;  
}
.side_element ul{ 
  display: flex; 
  flex-direction: column; 
  -webkit-box-align: center; 
  align-items: center; 
  margin: 0px; 
  padding: 0px; 
  list-style: none; 
}
.side_element ul li a{
  padding: 10px;
  display: inline-block; 
  text-decoration: none; 
  color: inherit; 
  position: relative; 
  transition:  all 0.25s cubic-bezier(0.645,0.045,0.355,1);
  width: 10px;
}
.side_element li a i {
  width: 18px; 
  height: 20px; 
  font-size: 20px;
}
.side_element li a i:hover {
color: #81b622;
}
.side_element li a i.icon {
  fill: none;
}
.side_element:after { 
  content: ""; 
  display: block; 
  width: 1px; 
  height: 90px; 
  margin: 0px auto; 
  background-color: grey; 
}
.right_element:after { 
  content: ""; 
  display: block; 
  width: 1px; 
  height: 90px; 
  margin: 0px auto; 
  background-color: grey;
}
.right_element div a { 
  margin: 20px auto; 
  padding: 10px;  
  font-size:12px;                   
  line-height: 18px; 
  letter-spacing: 0.1em; 
  -webkit-writing-mode: vertical-rl; 
  writing-mode: vertical-rl; 
  text-decoration: none;
}
.right_element div{
  display: flex; 
  flex-direction: column; 
  -webkit-box-align: center; 
  align-items: center; 
  position: relative;
}
</style>
