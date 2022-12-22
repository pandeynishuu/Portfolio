<template>
<template-view>
    <main>
        <div class="body">
            <!-- intro section -->
              <section class="intro-section">
                <intro-component/>
              </section>
              <!-- about section -->
              <section class="about-section">
                <about-view id="about"/>
              </section>
        </div>
    </main>
</template-view>
</template>

<script>
import TemplateView from "@/views/TemplateView";
import AboutView from '@/views/AboutView'
import IntroComponent from '@/components/IntroComponent'
// @ is an alias to /src

export default {
    name: "HomeView",
    components: {
        TemplateView,
        AboutView,
        IntroComponent
    },
};
</script>
