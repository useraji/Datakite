<script>
    let visible = false;

    function toggle(){
        visible = !visible
    };
</script>

<nav class="px-16 py-2 flex items-center justify-between shadow-md">
    <div class="flex items-center gap-5">
        <img src="/logo datakite.png" alt="datakite" class="w-14 py-3">
        <h1 class="text-md font-bold">DATAKITE FKIP UNTAN</h1>
    </div>

    <div class="lg:flex gap-5 md:hidden sm: hidden">
        <a href="/" class="text-xl font-bold text-orange-400">Beranda</a>
        <a href="/Survei" class="text-xl font-bold text-orange-400">Survei</a>
        <a href="/Database" class="text-xl font-bold text-orange-400">Database</a>
        <a href="/Riset" class="text-xl font-bold text-orange-400">Riset</a>
    </div>

    <i class="fas fa-bars text-xl px-3 py-1 border-2 border-orange-400 rounded-md cursor-pointer lg:hidden" on:click={toggle}></i>

</nav>

{#if visible}
<div class="flex flex-col items-center px gap-2 p-5 space-y-2 animate__animated animate__backInRight"> 
    <a href="/" class="text-xl font-bold text-orange-400">Beranda</a>
    <a href="/Survei" class="text-xl font-bold text-orange-400">Survei</a>
    <a href="/Database" class="text-xl font-bold text-orange-400">Database</a>
    <a href="/Riset" class="text-xl font-bold text-orange-400">Riset</a>
</div>
{/if}