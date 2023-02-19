<template>
    <div class="project-grid">
        <div class="project-item" v-for="project in projects">
            <img :src="project.mainImg" alt="project-cover-img"/>
            <div class="project-description">
                <h1>{{ project.title }}</h1>
                <p>{{ project.date }}</p>
            </div>
        </div>
    </div>
</template>

<style>
   .project-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    width: 100%;
    gap: 2rem;
   }
   .project-grid .project-item {
    padding: 2rem;
    background: var(--secondary-color);
    border-radius: 15px;
    display: flex;
    flex-direction: column;
    gap: 1rem;
   }
   .project-grid .project-item img {
    width: 100%;
    height: 300px;
    object-fit: cover;
    border-radius: 15px 15px 0 0;
   }
   .project-grid .project-item .project-description {
    display: flex;
    justify-content: space-between;
    align-items: center;
   }
   .project-grid .project-item .project-description h1 {
    width: 50%;
    font-size: 1.5rem;
   }
   .project-grid .project-item .project-description p {
    margin: 0;
   }
</style>

<script>
export default {
data() {
    return {
        projects: [
            {
                title: 'Juniper Research',
                date: 'Jan 2023',
                description: 'A large website build using Umbraco CMS',
                mainImg: '/src/assets/images/Portfolio/Juniper/juniper-landing.png',
                images: [
                    {url: '/src/assets/images/Portfolio/Juniper/juniper-landing.png'}
                ]
            },
            {
                title: 'Altro Flooring',
                date: 'March 2022',
                description: 'A large website build using Kentico CMS',
                mainImg: '/src/assets/images/Portfolio/altro/altro-landing.png',
                images: [
                    {url: '/src/assets/images/Portfolio/altro/altro-landing.png'}
                ]
            },
        ]
    }
}
}
</script>