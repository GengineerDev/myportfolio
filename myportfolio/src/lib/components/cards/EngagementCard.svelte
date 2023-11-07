<script>
	import Tag from "../elements/Tag.svelte";

    export let title = "Engagements";
    export let description = "Lorem ipsum dolor sit amet consectetur. Sem gravida dui nisi blandit nulla tincidunt tortor. Egestas nibh turpis arcu suscipit a in amet malesuada. Lacus quam quis odio erat varius adipiscing rutrum neque. Porta dui et amet urna. Orci sem ut egestas ridiculus orci augue non euismod.";
    export let tags = ['Mentoring', 'Voluntary'];
    export let imgPath = "";
    export let imgAlt = "Engagement Image";
</script>

<style>
    .engagement-card {
        display: grid;
        grid-template-columns: 45% 55%;
        padding: 40px 48px;
        border-radius: 40px;
        box-shadow: var(--shadow);
        margin-top: 40px;
    }

    .engagement-title {
        font-size: 32px;
    }

    .engagement-card-tags {
        margin: 10px 0;
        display: flex;
        gap: 13px;
    }

    .engagement-img {
        background: var(--gradient);
        width: 468px;
        max-width: 468px;
        height: 320px;
        max-height: 320px;
        border-radius: 20px;
        box-shadow: 4px 4px 40px -2px rgba(68, 68, 68, 0.10);
    }

    .engagement-content {
        display: flex;
        flex-direction: column;
        justify-content: center;
    }
</style>

<div class="engagement-card">
    <div class="engagement-img">
        {#if imgPath === ""}
            <p></p>
        {:else}
            <img src={imgPath} alt={imgAlt} />
        {/if}
    </div>
    <div class="engagement-content">
        <h2 class="gradient-text-background engagement-title">{title}</h2>
        <div class="engagement-card-tags">
            {#each tags as tag}
                <Tag size="small">{tag}</Tag>
            {/each}
        </div>
        <p class="body-3">{description}</p>
    </div>
    
    
</div>