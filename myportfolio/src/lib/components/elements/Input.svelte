<script>
    export let labelText = "label";
    export let name = "title";
    export let inputType = "text";
</script>

<div>
    <label for={name} class="body-1">{labelText}</label>
    <input type={inputType} id={name} name={name}/>
</div>


<style>
    label {
        font-family: unset;
        font-weight: unset;
        display: block;
        margin-bottom: 8px;
    }

    input {
        padding: 16px 24px;
        border: 1px solid #676767;
        width: 100%;
        background: var(--white);
        font-family: 'General Sans Regular', 'Times New Roman', Times, serif;
        font-size: 24px;
        font-weight: 400;
    }

    div {
        margin: 16px 0;
    }
</style>