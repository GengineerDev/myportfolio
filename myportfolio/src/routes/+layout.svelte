<script>
    import Navbar from "$lib/components/Navbar.svelte";
    import Footer from "$lib/components/Footer.svelte";
    import '../styles.css';
</script>

<Navbar />
<slot />
<Footer />