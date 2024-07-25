<script>
    export let name = "name";
    export let description = "description";
    export let url;
</script>

<!-- Item -->
<div class="flex flex-col md:flex-row justify-between">
    <div class="flex flex-col space-y-2">
        <div class="flex flex-row items-center space-x-3">
            <p>{name}</p>
            <div class="flex flex-row items-center space-x-3 overflow-x-scroll">
                <slot>icons</slot>
            </div>

        </div>

        <!-- Description -->
        <div class="flex flex-row space-x-2 md:hidden items-center">
            <p>{description}</p>
            <a href="{url}">
                <i class="fa-solid fa-arrow-up-right-from-square fa-xl"></i>
            </a>
        </div>
        <p class="hidden md:flex">{description}</p>
    </div>

    <!-- Link Icon -->
    <div class="hidden md:flex justify-center align-center items-center">
        <a href="{url}">
            <i class="fa-solid fa-arrow-up-right-from-square fa-xl"></i>
        </a>
    </div>
</div>