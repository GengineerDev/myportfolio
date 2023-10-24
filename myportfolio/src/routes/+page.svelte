<svelte:head>
    <title>David Genesis Pedeglorio - Portfolio</title>
</svelte:head>

<script>
    import '@fontsource-variable/space-grotesk';
    import AboutMe from '$lib/components/layouts/AboutMe.svelte';
	import TechStack from '$lib/components/layouts/TechStack.svelte';
    import BlogSection from '$lib/components/layouts/BlogSection.svelte';
	import ExperiencesSection from '$lib/components/layouts/ExperiencesSection.svelte';
	import CertificatesSection from '$lib/components/layouts/CertificatesSection.svelte';
	import ContactForm from '$lib/components/layouts/ContactForm.svelte';
</script>

<AboutMe />
<TechStack />
<ExperiencesSection />
<CertificatesSection />
<BlogSection />
<ContactForm />

