<script>
	import Button from "../elements/Button.svelte";

    export let title = "Default Title";
    export let paragraph = "Default Paragraph";
    export let buttonText = "Default Button Text";

</script>
<style>
    .action-card {
        border-radius: 20px;
        border: 4px solid var(--pantone-orange);
        padding: 56px 48px;
        width: 610px;
        max-width: 610px;
    }

    .action-card h2 {
        font-family: 'Space Grotesk Variable';
        font-size: 32px;
        font-weight: 700;
        margin-bottom: 16px;
    }

    .action-card p {
        margin-bottom: 24px;
    }

</style>

<div class="action-card">
    <h2 class="gradient-text-background">{title}</h2>
    <p class="body-3">{paragraph}</p>
    <Button size=''>{buttonText}</Button>
</div>