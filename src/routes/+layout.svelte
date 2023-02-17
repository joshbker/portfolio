<script lang="ts">
	import { onMount } from 'svelte';
    import '../app.css';
    import AOS from 'aos';

    onMount(() => {
		AOS.init();
	});
</script>

<div class="bg-[#18181B] min-h-screen min-w-screen flex justify-center">
    <div class="flex flex-col w-[70rem] mx-10 my-14 relative">
        <slot />
    </div>
</div>