<script>
  import { onMount } from 'svelte'

  onMount(async () => {
    const { Model } = await import('$src/components/threejs/coolers')
    new Model({
      dom: 'factory',
      model: '/models/factory_fan.glb'
    })
  })
</script>

<style>
  .factory {
    position: absolute;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
  }
</style>

<div class="factory" id="factory">
</div>