<script>
	import Button from "./ui/Button.svelte";

</script>
<header class="w-full h-[10vh] backdrop-blur-md flex justify-between items-center text-primary px-4 md:px-10">
    <nav class="hidden md:flex items-center justify-between gap-5 w-full text-sm">
        <a class="w-full" href="#about">About</a>
        <a class="w-full" href="#skills">Skills</a>
        <a class="w-full" href="#portfolio">Portfolio</a>
    </nav>
    <div class="w-full flex justify-center items-center">
        <h1 class="italic font-semibold w-fit h-fit border-b-4 border-accent px-4 rounded-full">Efandio</h1>
    </div>
    <a href="#footer" class="w-full">
    <div class="hidden w-full md:flex justify-center items-center">
        <Button label='Contact' style='rounded-full bg-primary' />
    </div>
    </a>
</header>