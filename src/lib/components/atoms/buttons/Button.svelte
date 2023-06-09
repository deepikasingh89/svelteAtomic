<script lang="ts">
    export let label: string;
    export let onClick: () => void;
</script>

<button class="ml-7 bg-red-600 px-6 py-2 text-white rounded-full hover:bg-blue-500 focus:outline-none focus:shadow-outline" on:click={onClick}>{label}</button>