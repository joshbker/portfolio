<script lang="ts">
    import experience from '$lib/data/experience.json';
    export let work: boolean;
</script>

<div class="border-[1px] border-[#3F3F46] bg-[#18181B] rounded-xl p-3 space-y-3 w-[28rem]">
    <div class="flex space-x-4 items-center p-3">
        {#if work}
            <svg class="h-5 fill-[#9898A5]" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><!--! Font Awesome Pro 6.2.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. --><path d="M448 96h-64V48C384 21.53 362.5 0 336 0h-160C149.5 0 128 21.53 128 48V96H64C28.65 96 0 124.7 0 160v256c0 35.35 28.65 64 64 64h384c35.35 0 64-28.65 64-64V160C512 124.7 483.3 96 448 96zM160 48C160 39.17 167.2 32 176 32h160C344.8 32 352 39.17 352 48V96H160V48zM480 416c0 17.64-14.36 32-32 32H64c-17.64 0-32-14.36-32-32V288h144v64c0 8.844 7.156 16 16 16h128c8.844 0 16-7.156 16-16V288H480V416zM208 336V288h96v48H208zM480 256H32V160c0-17.64 14.36-32 32-32h384c17.64 0 32 14.36 32 32V256z"/></svg>
        {:else}
            <svg class="h-5 fill-[#9898A5]" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Pro 6.2.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. --><path d="M448 368v-320C448 21.49 426.5 0 400 0h-320C35.82 0 0 35.82 0 80V448c0 35.35 28.65 64 64 64h368c8.844 0 16-7.156 16-16S440.8 480 432 480H416v-66.95C434.6 406.4 448 388.8 448 368zM32 80C32 53.49 53.49 32 80 32H96v352H64c-11.71 0-22.55 3.389-32 8.9V80zM384 480H64c-17.64 0-32-14.36-32-32s14.36-32 32-32h320V480zM400 384H128V32h272C408.8 32 416 39.17 416 48v320C416 376.8 408.8 384 400 384zM352 128H192C183.2 128 176 135.2 176 144S183.2 160 192 160h160c8.844 0 16-7.156 16-16S360.8 128 352 128zM352 224H192C183.2 224 176 231.2 176 240S183.2 256 192 256h160c8.844 0 16-7.156 16-16S360.8 224 352 224z"/></svg>
        {/if}
        <h3 class="text-white font-heading text-base">{work ? "Work" : "Education"}</h3>
    </div>
    <div>
        {#each (work ? experience.work : experience.education) as item}
            <a href="{item.info.link}" target="_blank" rel="noreferrer" class="flex space-x-6 w-full hover:bg-[#242429] transition-colors rounded-xl p-3">
                <div class="min-w-[3rem] w-[3rem] aspect-square bg-[#27272a] border-[1px] p-1.5 border-[#3F3F46] rounded-full">
                    <img src="/image/{item.info.logo}" alt="" class="rounded-full">
                </div>
                <div class="flex flex-col w-full">
                    <h4 class="text-white text-base">{item.name}</h4>
                    <div class="flex justify-between">
                        <p class="text-[#9898A5] text-sm">{item.role}</p>
                        <p class="text-[#777781] text-sm">{item.time.from} — {item.time.to}</p>
                    </div>
                </div>
            </a>
        {/each}
    </div>
</div>