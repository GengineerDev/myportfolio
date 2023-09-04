<style>
    .button {
        padding: 12px 24px;
        border-radius: 10px;
        background: var(--gradient, linear-gradient(166deg, #FF5800 -2.33%, #FF8A00 90.04%));
        box-shadow: 3px 3px 4px 0px rgba(255, 255, 255, 0.30) inset, -12px -12px 20px 8px #FFF, 12px 12px 20px 3px rgba(198, 175, 162, 0.30);
        color: var(--white);
        border: none;
    }

    .button-medium {
        padding: 10px 6px;
    }

</style>

<script>
    /**
	 * @type {string}
	 */
     export let size;
</script>

{#if size === "large"}
  <button class="button button-large">
    <p class="subheadings-1">
      <slot />
    </p>
  </button>
{:else if size === "medium"}
  <button class="button button-medium">        
    <label>
      <slot />
    </label>
  </button>
{:else}
  <button class="button">
    <slot />
  </button>
{/if}