<script setup>
    const route = useRoute();
    const message = computed(()=> `this is being shown from script tag ${ route.params.teamSlug }  ${ route.params.userId }` )
</script>


<template>
    <div>
        <h1>
            I'm from team {{ $route.params.teamSlug }}
            my user id is {{ $route.params.userId }}

            <br/>
            {{ message }}
        </h1>
    </div>
</template>

