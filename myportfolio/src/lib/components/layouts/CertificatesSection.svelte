<script>
	import CertificateCard from "../cards/CertificateCard.svelte";

</script>
<style>
    #certificates {
        border-top: 1px solid var(--pantone-orange);
        border-bottom: 1px solid var(--pantone-orange);
        padding: 40px 0;
        
    }

    #certificates h2 {
        margin-bottom: 16px;
    }
</style>

<section id="certificates">
    <center>
        <h2 class="gradient-text-background">&lt; CERTIFICATES &gt;</h2>
    </center>
    <div class="card-container">
        <CertificateCard />
        <CertificateCard />
        <CertificateCard />
    </div>
</section>