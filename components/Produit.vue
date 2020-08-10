<template>
    <div class="card text-white bg-dark mb-3" style="max-width: 18rem;">
        <div class="card-header">{{ nom }}</div>
        <div class="card-body">
            <p class="card-text">Price : {{ prix }}</p>
            <button 
                v-if="role == 'commander'" 
                @click="$emit('commande', nom, prix)" 
                class="btn btn-success">
                Order now
            </button>
        </div>
    </div>
</template>

<script>
export default {
    name: "Produit",
    props: ["nom", "prix", "role"]
}
</script>