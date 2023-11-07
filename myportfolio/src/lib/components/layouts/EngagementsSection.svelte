<script>
	import EngagementCard from "../cards/EngagementCard.svelte";
	import Tag from "../elements/Tag.svelte";

</script>

<style>
    .engagement-p {
        margin: 16px 0;
    }

    .engagements-tags {
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 12px;
        flex-wrap: wrap;
    }

    .engagements-header {
        margin-top: 160px;
    }
</style>

<section id="engagements">
    <center>
        <h2 class="gradient-text-background engagements-header">&lt; OTHER ENGAGEMENTS &gt;</h2>
        <p class="subheadings-2 gradient-text-background engagement-p">Here are my other engagements aside from web development.</p>
    </center>
    <div class="engagements-tags">
        <Tag size="small">ALL</Tag>
        <Tag size="small">Mentoring</Tag><Tag size="small">Organizations</Tag>
        <Tag size="small">Modeling</Tag>
        <Tag size="small">Youth Organizations</Tag>
    </div>
    <EngagementCard />
    <EngagementCard />
    <EngagementCard />
</section>