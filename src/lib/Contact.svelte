<div class="max-w-sm mb-6">
    <h4>{name} {#if title} - {title}{/if}</h4>
    <a class="block text-slate-600" href="tel:+420{tel.replace(/\s/g, '')}">{tel}</a>
    {#if email}<a class="block text-slate-600" href="mailto:{email}">{email}</a>{/if}
</div>

<script>
    export let name;
    export let title;
    export let tel;
    export let email = "";
</script>