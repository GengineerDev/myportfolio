<script>
	import Button from '../elements/Button.svelte';
import Input from '../elements/Input.svelte';
	import Tag from '../elements/Tag.svelte';
</script>

<div class="contact-form">
	<h2 class="gradient-text-background">Interested in working together?</h2>
	<p class="body-3 p-subheading">
		Are you looking for a skilled and dedicated freelancer to help bring your project to life,
		whether it's a website, mobile app, software, game, or something else entirely? I'm here and
		eager to work with you!
	</p>
	<div class="project-type">
		<p class="body-1 project-type" id="project-type">Project Type</p>
		<div>
			<Tag size="small">Website</Tag>
			<Tag size="small">Mobile App</Tag>
			<Tag size="small">Software</Tag>
			<Tag size="small">Game</Tag>
		</div>
	</div>
	<div />
	<Input labelText="Title" name="title" />
	<div class="two-fields">
		<Input labelText="Name" name="name" />
		<Input labelText="Email" name="email" inputType="email" />
	</div>
    <Input labelText="Project Description" name="project description" textarea={true} helperText="Feel free to describe your vision."/>
    <Button size="large">Let&#39;s work together</Button>
</div>

<style>
	.contact-form {
		padding: 72px 140px;
		border: 4px solid var(--pantone-orange);
		border-radius: 0px 90px 0px 0px;
		margin-bottom: 95px;
		margin: inherit;
		box-shadow: var(--shadow);
	}

	.p-subheading {
		padding: 10px 0px;
	}

	.contact-form > div {
		margin-top: 16px;
	}

	.project-type {
		display: grid;
		grid-template-columns: 20% 80%;
		align-items: center;
	}

	#project-type {
		display: unset;
		color: var(--main-colors-gray-4);
	}

	.two-fields {
		display: grid;
		grid-template-columns: 1fr 1fr;
		grid-gap: 25px;
	}
</style>
