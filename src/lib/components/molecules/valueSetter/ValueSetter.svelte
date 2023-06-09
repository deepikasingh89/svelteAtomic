<script lang="ts">
  import Button from "../../atoms/buttons/Button.svelte";
  export let onIncrease: () => void;
  export let onDecrease: () => void;
  export let onReset: () => void;
</script>

<Button label="+" onClick={onIncrease} />
<Button label="-" onClick={onDecrease} />
<Button label="Reset" onClick={onReset} />
