<script>
    import Tile from "$lib/component/Tile.svelte";
    import tailwindLogo from '$lib/image/tailwindcss-mark.svg';
    import svelteLogo from '$lib/image/svelte.png';
    import tsLogo from '$lib/image/ts.png';
    import jsLogo from '$lib/image/js.png';
    import javaLogo from '$lib/image/java.png';
    import figmaLogo from '$lib/image/figma.png';
    import mongoLogo from '$lib/image/mongodb.png';
    import jetbrainsLogo from '$lib/image/jetbrains.png';
</script>

<div class="">
    <div>
        <div class="-translate-x-[9rem] translate-y-[2.75rem]">
            <Tile logo={svelteLogo} name="Svelte" shadowColor={[255, 62, 0]} />
        </div>
        <div class="">
            <Tile logo={tailwindLogo} name="Tailwind" shadowColor={[56, 189, 248]} />
        </div>
        <div class="translate-x-[9rem] -translate-y-[2.75rem]">
            <Tile logo={figmaLogo} name="Figma" shadowColor={[10, 207, 131]} />
        </div>
        <div class="translate-x-[18rem] -translate-y-[5.5rem]">
            <Tile logo={javaLogo} name="Java" shadowColor={[240, 63, 51]} />
        </div>
    </div>
    <div class="translate-y-[6.5rem] translate-x-[6rem]">
        <div class="-translate-x-[9rem] translate-y-[2.75rem]">
            <Tile logo={mongoLogo} name="MongoDB" shadowColor={[10, 207, 131]} />
        </div>
        <div class="">
            <Tile logo={jsLogo} name="JavaScript" shadowColor={[240, 219, 79]} />
        </div>
        <div class="translate-x-[9rem] -translate-y-[2.75rem]">
            <Tile logo={jetbrainsLogo} name="JetBrains" shadowColor={[254, 49, 93]} />
        </div>
        <div class="translate-x-[18rem] -translate-y-[5.5rem]">
            <Tile logo={tsLogo} name="TypeScript" shadowColor={[49, 120, 198]} />
        </div>
    </div>
</div>