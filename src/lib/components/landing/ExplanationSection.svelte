<script>
    import nuitInfo from '$lib/assets/nuitInfo.svg';
    const sections = [
        {
            image: nuitInfo,
            text: "La Nuit de l’Info est un événement annuel qui rassemble des étudiants, des professionnels, et des passionnés d’informatique et d’innovation pour relever ensemble des défis numériques. Pendant 12 heures consécutives, les équipes travaillent sur des projets interactifs, éducatifs, ou techniques en réponse à des problématiques proposées par des entreprises ou des organisations partenaires."
        },
        {
            image: "https://upload.wikimedia.org/wikipedia/commons/3/3f/Race_for_Water_Foundation_-_Logo.svg",
            text: "Race for Water est une fondation suisse dédiée à la protection de l’Océan et des ressources aquatiques. Depuis plus de dix ans, cette organisation innovante s’engage dans des initiatives concrètes pour sensibiliser le public, mobiliser les décideurs, et promouvoir des solutions durables face aux grands défis environnementaux."
        }
    ];
</script>

<section>
    <div class="flex justify-center mx-auto border-t pt-12 max-w-screen-lg">
        <h2 class="text-5xl font-medium">Explications du projet</h2>
    </div>
    {#each sections as section, index}
        <div class="grid max-w-screen-xl px-4 py-8 mx-auto lg:gap-8 xl:gap-16 lg:py-12 lg:grid-cols-12 ">
            {#if index % 2 === 1}
                <div class="mr-auto place-self-center lg:col-span-9">
                    <p class="font-light text-zinc-500 text-justify md:text-lg lg:text-2xl dark:text-zinc-400">{section.text}</p>
                </div>
                <div class="hidden lg:mt-0 lg:col-span-3 lg:flex">
                    <img src={section.image} alt="mockup" class="w-full">
                </div>
            {:else}
                <div class="hidden lg:mt-0 lg:col-span-3 lg:flex">
                    <img src={section.image} alt="mockup" class="w-full">
                </div>
                <div class="mr-auto place-self-center lg:col-span-9">
                    <p class="font-light text-zinc-500 text-justify md:text-lg lg:text-2xl dark:text-zinc-400">{section.text}</p>
                </div>
            {/if}
        </div>
    {/each}
</section>