<script>
    import Navbar from "$lib/components/layouts/Navbar.svelte";
    import Footer from "$lib/components/layouts/Footer.svelte";
    import '../styles.css';
</script>

<link rel="stylesheet" href="/fonts/fonts.css">

<Navbar />
<slot />
<Footer />