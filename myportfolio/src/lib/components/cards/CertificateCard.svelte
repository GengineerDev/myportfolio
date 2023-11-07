<script>
    export let title = "Certificate Title";
    export let date = "Date";
    // export let imgPath = "/icons/TENTEN.png";
</script>

<style>
    .certificate-pic {
        width: 384px;
        max-width: 384px;
        height: 227px;
        max-height: 227px;
        margin-bottom: 8px;
        border-radius: 20px;
        border: 2px solid var(--pantone-orange);
        opacity: 0.44;
    }
</style>

<div class="certificate-card">
    <div class="certificate-pic"></div>
    <center>
        <p class="body-1 gradient-text-background">
            {title}<br />
            {date}
        </p>
    </center>
</div>
