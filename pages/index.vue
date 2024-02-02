<script setup lang="ts">

const content = {
    technologies: [
        {
            title: "Frontend Development",
            content: "Crafting interactive UIs with Dart, HTML5, CSS3, JavaScript; proficient in Flutter, Nuxt, Vue.js."
        },
        {
            title: "Backend Development",
            content: "Developing robust server-side solutions using Node.js, Python; managing databases with MongoDB, MySQL."
        },
        {
            title: "AI and Machine Learning",
            content: "Expert in creating deep learning models, generative AI, and predictive analytics. Skilled in data visualization, transforming complex data into clear, engaging visual stories."
        },
        {
            title: "Other Tech",
            content: "Version control with Git; leveraging Docker, Kubernetes for efficient deployment; cloud solutions via AWS, Azure."
        },
        {
            title: "Network Design and Construction",
            content: "Specialized in Omada solutions and public network infrastructure; adept in designing, implementing, and securing large-scale networks for public use."
        }
    ] 
}
</script>

<template>
    <div class="d-flex flex-column ga-6">
        <!-- Hero -->
        <section> 
            <VCard>
                <VCardText>
                    Hey I'm a
                    <h4 class="text-h4">Full Stack Web Developer</h4>
                    <div>
                        Hello, I'm Gabriel Biler, a dedicated Developer and Data Science student. I specialize in crafting 
                        elegant solutions in web, mobile, and desktop application development, and possess a keen interest 
                        in network architecture.
                    </div>
                    <div>
                        <VBtn href="mailto: me@gabsbiler.com">
                            Contact Me
                        </VBtn>
                    </div>
                </VCardText>
            </VCard>
        </section>

        <section>
            <VCard>
                <VCardText>
                    <h5 class="text-h5">
                        Services I can help you with...
                    </h5>
                    <div class="d-flex ga-2" style="max-width: 40rem;">
                        <div>
                            Full Stack Development
                        </div>
                        <div>
                            Frontend Dev.
                        </div>
                        <div>Backend Dev.</div>
                        <div>
                            Dev Ops.
                        </div>
                        <div>Network Design & Construction</div>
                    </div>
                </VCardText>
            </VCard>
        </section>
        <!-- Feature Project -->
        <section style="background-color: white;">
            <VCard>
                <VCardText>
                    <h5 class="text-h5">
                        <em>" I focus on delivering high-quality, user-centric applications."</em>
                    </h5>
                    <div>
                        *sample projects*
                    </div>
                </VCardText>
            </VCard>
            
        </section>

        <!-- Technologies -->
        <section>
            <VRow>
                <VCol 
                    cols="4" 
                    v-for="techs in content.technologies"
                >
                    <VCard 
                        :title="techs.title"
                        style="min-height: 10rem;"
                    >
                        <VCardText>
                            {{techs.content}}
                        </VCardText>
                    </VCard>
                </VCol>
            </VRow>
        </section>
    </div>
</template>