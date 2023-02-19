<script setup>
    import Navigation from './components/navigation.vue'
    import Projects from './components/projects.vue'
</script>

<template>
  <div class="container my-5">
    <div class="bg-img"><img src="./assets/images/BG.png"/></div>
    <header>
         <Navigation></Navigation>
    </header>

    <div class="main">
            <div class="splash">
                <div class="profile">
                    <a class="profile-img"><img src="./assets/images/image3.png"/></a>
                    <div class="info">
                        <div class="name">thomas (tommy) pippard</div>
                        <div class="about">Graphic Designer/Web Developer</div>
                        <div class="link">Follow Me! <ion-icon name="caret-forward-outline"></ion-icon></div>
                    </div>
                </div>
                <div class="description">
                    <p>A design wizard voyaging into the metaverse. I tell the story through my design and illustrations. I spent most of my time designing for brands and creating open-source design resources.</p>
                    <div class="bot">

                    </div>
                </div>
                
            </div>
            <div class="api">
                <div class="clock">
                    <img class="accent" src="./assets/images/tape1.svg"/>
                    
                </div>
                <div class="steam">
                    <img class="accent" src="./assets/images/tape2.svg"/>
                    <ion-icon name="logo-steam"></ion-icon>
                </div>
            </div>
            <div class="projects">
                <h2>Featured Projects</h2>
                <Projects></Projects>
                    </div>
                </div>
    <footer>

    </footer>
  </div>
</template>

<style scoped>

</style>
