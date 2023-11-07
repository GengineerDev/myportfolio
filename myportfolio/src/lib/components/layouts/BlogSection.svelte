<style>
    div {
        margin-top: 24px;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
        margin-bottom: 160px;
    }
</style>

<script>
    import ActionCard from "../cards/ActionCard.svelte";
</script>

<div>
    <ActionCard 
        title="Read my blogs."
        paragraph="Lorem ipsum dolor sit amet consectetur. Sem gravida dui nisi blandit nulla tincidunt tortor. Egestas nibh turpis arcu suscipit a in amet malesuada. Lacus quam quis odio erat varius adipiscing rutrum neque."
        buttonText = "My Blog Website"
    />
    <ActionCard 
        title="Watch my videos."
        paragraph="Lorem ipsum dolor sit amet consectetur. Sem gravida dui nisi blandit nulla tincidunt tortor. Egestas nibh turpis arcu suscipit a in amet malesuada. Lacus quam quis odio erat varius adipiscing rutrum neque."
        buttonText = "My YouTube Channel"
    />
</div>
