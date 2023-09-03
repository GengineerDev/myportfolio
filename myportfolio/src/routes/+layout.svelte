<script>
    import Navbar from "$lib/components/Navbar.svelte";
    import Footer from "$lib/components/Footer.svelte";
    import '../styles.css';
</script>

<link rel="stylesheet" href="/fonts/fonts.css">

<Navbar />
<slot />
<Footer />