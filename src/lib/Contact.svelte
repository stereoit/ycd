<div class="max-w-sm mb-6">
    <h4 class="truncate">{name} {#if title} - {title}{/if}</h4>
    <a class="block text-slate-900 font-medium" href="tel:+420{tel.replace(/\s/g, '')}">{tel}</a>
    {#if email}<a class="block text-slate-600 text-sm" href="mailto:{email}">{email}</a>{/if}
</div>

<script>
    /** @type {{name: any, title: any, tel: any, email?: string}} */
    let {
        name,
        title,
        tel,
        email = ""
    } = $props();
</script>