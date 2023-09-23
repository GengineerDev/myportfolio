<script>
	import Tag from "../elements/Tag.svelte";
</script>

<style>
    .tech-stack {
        padding: 0 120px;
        margin-top: 64px;
    }
    
    .tech-stack-container {
        display: flex;
        padding: 0px 120px;
        justify-content: center;
        align-items: center;
        align-content: center;
        gap: 12px;
        align-self: stretch;
        flex-wrap: wrap;
    }

    .tech-stack h2 {
        margin-bottom: 16px;
    }
</style>

<div class="tech-stack">
    <center>
        <h2 class="gradient-text-background">TECH STACK</h2>
    </center>
    <div class="tech-stack-container">
        <Tag>ALL</Tag>
        <Tag>Frontend Development</Tag>
        <Tag>Backend Development</Tag>
        <Tag>Mobile App Development</Tag>
        <Tag>General Programming</Tag>
        <Tag>Machine Learning</Tag>
        <Tag>Toolkit</Tag>
    </div>
    
</div>
