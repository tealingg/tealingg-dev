<script lang="ts">

import Particles, { particlesInit } from "@tsparticles/svelte";
import { loadSlim } from "@tsparticles/slim";

import ContactCard from "$lib/ContactCard.svelte";

void particlesInit(async (engine) => {
    await loadSlim(engine)
})

</script>

<Particles
    id="tsparticles"
    url="particles.json"
/>

<div class="flex relative gap-12 flex-col z-10 min-h-screen min-w-screen justify-center items-center">
    <div class="transition ease-linear duration-100 bg-zinc-800 text-4xl font-bold p-6 border-transparent border-4 hover:border-cyan-500">
        <h1>tealingg<span class="text-neutral-500">.dev</span></h1>
    </div>
    <div class="flex flex-row flex-wrap justify-center max-w-3xl gap-8">
        <ContactCard name="Discord" icon="fa-brands fa-discord" colour="#7785CC" link="https://discord.com" />
        <ContactCard name="GitHub" icon="fa-brands fa-github" link="https://github.com/tealingg" />
        <ContactCard name="Twitch" icon="fa-brands fa-twitch" colour="#9146FF" link="https://twitch.tv/tealingg" />
        <ContactCard name="YouTube" icon="fa-brands fa-youtube" colour="#FF0000" link="https://youtube.com/@tealingg" />
    </div>
    <div class="transition ease-linear duration-100 bg-zinc-800 p-4 border-transparent border-4 hover:border-cyan-500">
        <h1 class="text-neutral-500">more coming soon...</h1>
    </div>
</div>