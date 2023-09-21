<style>
    .button {      
      padding: 12px 24px;
      border-radius: 10px;
      background: var(--gradient);
      box-shadow: 3px 3px 4px 0px rgba(255, 255, 255, 0.30) inset, -12px -12px 20px 8px #FFF, 12px 12px 20px 3px rgba(198, 175, 162, 0.30);
      color: var(--white);
      border: none;
      cursor: pointer;
    }

    .button-medium {
      padding: 10px 6px;
    }

    .button:hover {
      background: var(--pantone-orange);
    }

    .button:active {
      background: var(--gradient_yellow-orange, linear-gradient(265deg, #FFC635 5.6%, #FF7A00 118.86%));
    }

    .with-arrow {
      display: flex;
      gap: 8px;
    }

    .with-arrow label {
      cursor: pointer;
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
  <button class="button button-medium">
    <div class="with-arrow">
      <label>
        <slot />
      </label>      
      <img src="/icons/arrow_outward.svg" alt="Arrow Right" height="24px" />
    </div>
    
  </button>
{/if}