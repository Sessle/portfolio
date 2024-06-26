<script>
    export let name = "name";
    export let description = "description";
    export let url;
</script>

<!-- Item -->
<div class="flex flex-row justify-between">
    <div class="flex flex-col space-y-2">
        <div class="flex flex-row items-center space-x-3">
            <p>{name}</p>
            <slot>icons</slot>
        </div>

        <!-- Description -->
        <p>{description}</p>
    </div>

    <!-- Link Icon -->
    <div class="flex justify-center align-center items-center">
        <a href="{url}">
            <i class="fa-solid fa-arrow-up-right-from-square fa-xl"></i>
        </a>
    </div>
</div>