<script setup>
import Logos1 from './icons/logos1.vue';
defineProps({
    msg: {
        type: String,
        required: true,
    },
});
</script>

<template>
    <WelcomeItem>
        <template #icon>
            <Logos1 />
        </template>
        <template>
            <div class="greetings">
                <h1 class="yellow">{{ msg }}</h1>
                <h3>
                    DeltCrosX Web Port
                    <a target="__blank" href="https://dotnet.microsoft.com/en-us/languages/csharp">Microsoft C#</a>, 
                    <a target="__blank" href="https://dotnet.microsoft.com/en-us">Microsoft DOTNET</a>, 
                    <a target="__blank" href="https://www.iso.org/standard/74528.html">C</a>, 
                    <a target="__blank" href="https://www.isocpp.org">C++</a>, 
                    <a target="__blank" href="https://www.php.net">PHP</a>, 
                    <a target="__blank" href="https://html.spec.whatwg.org">HTML</a>, 
                    <a target="__blank" href="https://www.w3.org/Style/CSS/Overview.en.html">CSS</a>, 
                    <a target="__blank" href="https://nodejs.org">JavaScript</a>, 
                    <a target="__blank" href="https://www.iso.org/standard/63555.html">SQL</a>, 
                    <a target="__blank" href="https://www.python.org">Python</a>.
                </h3> 
            </div>
        </template>
    </WelcomeItem>
</template>

<style scoped>

h1 {
    font-weight: 500;
    font-size: 2.6rem;
    top: -10px;
}

h3 {
    font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
    text-align: center;
}

@media(min-width: 1100) {
    .greetings h1,
    .greetings h3 {
        text-align: center;
    }
}

</style>

<script>
export default defineComponent({
    setup() {
        name: mainpageVue
    },
})
</script>
