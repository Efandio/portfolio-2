
<script>
    const portfolio = [
        {
            title: 'Task & Notes Management',       
            link: 'https://www.figma.com/design/4KtcgFp9v0fmEc8vEXo3u0/Zendo?node-id=57-761&t=i8UjUIU5YV3pODS9-1',
            img: '/porto1.png',
        },
        {
            title: 'Landing Page',       
            link: 'https://www.figma.com/design/9LSjcMqLXDL9vv6sAS0cih/Landing-Page?node-id=0-1&t=cVGreQ1D3pMtbw8c-1',
            img: '/porto2.png',
        },
        {
            title: 'My Personal Portfolio Website',       
            link: 'https://www.figma.com/design/hwCFEiPcWRcUpukRdTe1M5/Personal-Portfolio?node-id=0-1&t=iOlvf3xA5JAT0HAL-1',
            img: '/porto3.png',
        },
    ]
</script>

<section id="portfolio" class="w-full h-full flex flex-col gap-3 md:pt-30 px-4 md:px-10">
    <h3 class="text-accent font-semibold italic text-xl border-b border-accent w-fit pr-4">
        Portfolio
    </h3>

    <div class="w-full h-full grid grid-cols-1 md:grid-cols-3 gap-10">
        {#each portfolio as porto }
            <div class="w-full h-fit flex flex-col border border-primary rounded-lg pb-4 gap-2">
                <div class="w-full h-full aspect-video">
                    <img class="rounded-md w-full h-full object-center" src={porto.img} alt="">
                </div>
                <div class="flex flex-col gap-1 px-2">
                    <h4 class="text-primary italic font-semibold">
                        {porto.title}
                    </h4>
                    <a href={porto.link} class="text-accent text-xs">
                        Click this to see design source [Figma]
                    </a>
                </div>
            </div>
        {/each}
    </div>
</section>