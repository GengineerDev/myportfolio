<script>
	import CompanyCard from "../cards/CompanyCard.svelte";

</script>

<style>

    #experiences {
        margin: 80px 0;
    }
</style>

<section id="experiences">
    <center>
        <h2 class="gradient-text-background">&lt; EXPERIENCES &gt;</h2>
        <p class="subheadings-2 gradient-text-background">Here are the companies I've worked with.</p>
    </center>
    <div class="card-container">
        <CompanyCard
            imgPath="/icons/TENTEN.png"
            companyName="Tenten's Academy Online Tutorial"
        />
        <CompanyCard
            imgPath="/icons/FWDP.png"
            companyName="Filipino Web Development Peers"
        />
        <CompanyCard
            imgPath="/icons/PlantBox.jpg"
            companyName="Movement for Sustainable Communities"
        />
        <CompanyCard
            imgPath="/icons/iPhiTech.jpg"
            companyName="iPhiTech IT and Digital Solutions"
        />
        <CompanyCard
            imgPath="/icons/Pixel8.jpg"
            companyName="Pixel8 Web Solutions & Consultancy Inc"
        />
        <CompanyCard
            imgPath="/icons/ChefWorks.png"
            companyName="Chefworks Philippines"
        />
    </div>
    
</section>