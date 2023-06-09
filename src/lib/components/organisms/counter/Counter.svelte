<script lang="ts">
    import countStore from "../../../../store/stores";
    import ValueSetter from "../../molecules/valueSetter/ValueSetter.svelte";
</script>
<div class="p-2 lg::w-11/12 w-full">
  <div class="bg-blue-600 rounded p-4 text-center text-white">
    <h1>Global count is: {$countStore}!</h1>
  </div>
</div>

<ValueSetter
    onIncrease={() => ($countStore = $countStore + 1)}
    onDecrease={() => ($countStore = $countStore - 1)}
    onReset={() => ($countStore = 0)} />