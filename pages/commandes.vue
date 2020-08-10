<template>
    <div>
        <h1 class="display-1">SHOP</h1>

        <h2>Available Products</h2>
        <div class="card-deck">
            <Produit v-for="produit in produits" role="commander" v-bind:nom="produit.nom" :prix="produit.prix" v-on:commande="ajouterProduit" />
        </div>

        <h2>Ordered Products</h2>
        <div class="card-deck">
            <Produit v-for="produit in commandes" role="affichage" v-bind:nom="produit.nom" :prix="produit.prix"/>
        </div>
        <footer>
            <nuxt-link class="homeback" to="/">Home</nuxt-link>
        </footer>
    </div>
</template>

<script>
import Produit from '@/components/Produit.vue'
export default {
    components: {
        Produit
    },
    data () {
        return {
            produits: [
                { nom: 'Green Pill', prix: 3.0 },
                { nom: 'Red Pill', prix: 2.0 },
                { nom: 'Blue Pill', prix: 1.5 },
                { nom: 'Purple Pill', prix: 2.0}
            ],
            commandes: [
                // { nom: 'Pepsi', prix: 1.5}
            ]
        }
    },
    methods:{
        ajouterProduit(nom, prix) {
            this.commandes.push({nom: nom, prix: prix})
        }
    }
}
</script>

<style scoped>

.homeback {
    text-align: center;
    display: flex;
    text-decoration: none;
}
</style>