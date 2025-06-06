<script>
	import Button from "./ui/Button.svelte";

</script>

<section class="w-full h-90 rounded-full border-b-5 border-accent flex flex-col justify-center items-center gap-10 px-4 md:px-10">
    <div class="flex flex-col justify-center items-center gap-0.5 w-full">
        <h1 class="text-text text-4xl font-bold">UI/UX Designer</h1>
        <h2 class="text-primary text-center">
            Who
            <span class="text-accent">Design Experinces</span>
            with
            <span class="text-accent">Frontend Understanding</span>
        </h2>
    </div>

    <div class="flex items-center justify-between w-80 gap-5 md:w-120 md:gap-10">
        <Button label='See my works' style='rounded-md bg-transparent border border-primary text-primary font-normal hover:bg-hover hover:text-background transition ease' />
        <Button label='Lets Talk' style='rounded-md bg-primary hover:bg-primary/90' />
    </div>
</section>