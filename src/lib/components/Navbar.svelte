<script lang="ts">
    import { menuItems } from "../config"
</script>

<nav class="fixed top-0 left-0 right-0 text-white border-b border-zinc-800">
    <div class="px-8 py-6 md:p-10 lg:p-12 flex items-center gap-12 font-semibold">
        <a class="flex items-center gap-0" href="/">
            <span class="p-1.5 text-black/80 bg-white border border-transparent rounded-l">Mzizi</span>
            <span class="p-1.5 border border-current rounded-r">Agency</span>
        </a>
        <ul class="hidden md:flex md:items-center md:gap-8 mx-auto">
            {#each menuItems as menuItem}
                <li>
                    <a class="hover:text-emerald-500" href={menuItem.href}>
                        {menuItem.title}
                    </a>
                </li>
            {/each} 
        </ul>
        <div class="w-max ml-auto flex items-center gap-12">
            <button 
                class="px-3 py-2.5 border rounded-lg border-current hover:text-emerald-500"
            >
                Talk to us
            </button>
        </div>
    </div>
    <div class="absolute bg-black/50">
    
    </div>
</nav>

