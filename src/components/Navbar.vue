<script>
    export default {
        props: ['href', 'name', 'fa_icons']
    }
</script>

<template>
    <a :href="href" class="hidden lg:[display:block] text-slate-800 transition ease-in-out hover:text-slate-400 duration-300 [margin:0.25em]"> {{ name }} </a>
    <a :href="href" class="[display:block] lg:hidden text-slate-800 transition ease-in-out hover:text-slate-400 duration-300"> <i :class="fa_icons"></i> </a>
</template>