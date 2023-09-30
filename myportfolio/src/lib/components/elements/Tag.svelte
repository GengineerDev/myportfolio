<script>
    export let size = "primary";
    let clicked = false;
  
    function handleClick() {
      clicked = true;
    }
  </script>
  
  <style>
    .tag, .tag label {
      cursor: pointer;
    }
  
    .tag {
      padding: 16px 24px;
      border-radius: 90px;
      border: 4px solid var(--pantone-orange);
      width: auto;
      background: transparent;
    }
  
    .small-tag {
      padding: 8px 16px;
    }
  
    .tag-clicked {
      background: var(--gradient);
    }
  
    .label-clicked {
      color: var(--white);
    }
  </style>
  
{#if size === "primary"}
<button class="tag" class:tag-clicked={clicked} on:click={handleClick}>
    <label class={clicked ? " label-clicked" : "gradient-text-background"}>
        <slot />
    </label>   
</button>
{:else if size === "small"}
<button class="tag small-tag" class:tag-clicked={clicked} on:click={handleClick}>
    <label class={clicked ? " label-clicked" : "gradient-text-background"}>
        <slot />
    </label> 
</button>
{/if}