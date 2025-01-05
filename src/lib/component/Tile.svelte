<script lang="ts">
    export let logo: string;
    export let name: string;
    export let shadowColor: number[];
</script>

<div class="group hover:-translate-y-2.5 transition-transform">
    <div class="relative logo-rotate">
        <div class="absolute w-36 h-36 rounded-3xl translate-y-1.5 -translate-x-1.5" style="box-shadow:-70px 70px 65px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.07), -30px 30px 30px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.06), -15px 15px 15px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.05), -10px 10px 8px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.04), -4px 4px 4px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.03), -2px 2px 2px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.02);">
        </div>
        <div class="absolute w-36 h-36 rounded-3xl translate-y-1.5 -translate-x-1.5 opacity-0 group-hover:opacity-100 transition-opacity" style="box-shadow:-70px 70px 65px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.07), -30px 30px 30px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.06), -15px 15px 15px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.05), -10px 10px 8px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.04), -4px 4px 4px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.03), -2px 2px 2px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.02);">
        </div>
        <div class="absolute w-36 h-36 opacity-70 rounded-3xl translate-y-1.5 -translate-x-1.5 bg-white">
        </div>
        <div class="absolute w-36 h-36 rounded-3xl flex transition-opacity items-center justify-center p-10 bg-[#ECECEC] group-hover:bg-white">
            <img src={logo} alt="" class="h-full opacity-80 group-hover:opacity-100 transition-opacity">
            <div class="absolute text-center translate-y-1.5 -translate-x-1.5 rounded-3xl bottom-2 py-2 px-3 opacity-0 group-hover:opacity-100 transition-opacity bg-[#ECECEC]" style="box-shadow:-70px 70px 65px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.07), -30px 30px 30px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.06), -15px 15px 15px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.05), -10px 10px 8px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.04), -4px 4px 4px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.03), -2px 2px 2px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.02);">
                <h1 class="font-bold text-base text-[#ECECEC] group-hover:text-white">{name}</h1>
            </div>
            <div class="absolute text-center rounded-3xl bottom-2 py-2 px-3 opacity-0 group-hover:opacity-100 transition-opacity bg-[#ECECEC] group-hover:bg-white" style="box-shadow:-70px 70px 65px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.07), -30px 30px 30px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.06), -15px 15px 15px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.05), -10px 10px 8px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.04), -4px 4px 4px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.03), -2px 2px 2px rgb({shadowColor[0]} {shadowColor[1]} {shadowColor[2]} / 0.02);">
                <h1 class="font-bold text-base text-[#19191C]">{name}</h1>
            </div>
        </div>
    </div>
</div>