<script>
    export let name = "Name";
    export let icon = "fa-regular fa-user";
    export let accountName = "@tealingg";
    export let colour = "#06b6d4";
    export let link = "";
</script>

<style>

#card:hover {
    border-color: var(--border-color);
}

</style>

<a id="card" class="flex flex-row transition items-center gap-6 min-w-56 ease-linear duration-100 bg-zinc-800 px-6 py-4 border-transparent border-2" style="--border-color: {colour}" href={link} target="_blank">
    <i class="text-3xl {icon}" style="color: {colour}"></i>
    <div class="flex flex-col">
        <p class="font-bold text-xl" style="color: {colour}">{name}</p>
        <p>{accountName}</p>
    </div>
</a>