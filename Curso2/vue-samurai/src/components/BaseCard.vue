<template>
    <div>
        <b-col md="3">
            <b-card 
            :title="nome" 
            img-src="https://picsum.photos/id/237/200/300" 
            img-alt="Curso de Vue.JS" 
            style="max-width: 20rem;" 
            img-top 
            tag="article" 
            class="mb-2">
                <b-card-text>
                    Lorem ipsum dolor sit amet
                </b-card-text>
                <b-button variant="primary">Comprar</b-button>
            </b-card>
        </b-col>
    </div>
</template>

<script>
export default {
  name: "BaseCard",
  props: {
    nome: {
        type: String,
        required: true
    }
},
}
</script>