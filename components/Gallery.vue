<template>
    <b-carousel
        :autoplay="true"
         with-carousel-list
        :indicator="true"
        :pause-info="false"
        :arrow="false"
        class=" rounded-lg overflow-hidden cursor-pointer"
        :interval="2000"
        >
        <b-carousel-item v-for="(item, i) in items" :key="i">
            <figure  class="image">
                <img :src="item.image">
            </figure>
        </b-carousel-item>
        <span v-if="gallery" @click="switchGallery(false)" class="modal-close is-large"/>
        <!-- <template slot="list" slot-scope="props">
            <b-carousel-list
                :arrow="false"
                :repeat="true"
                v-model="props.active"
                :data="items"
                :config="al"
                :refresh="true"
                @switch="props.switch($event, false)"
                as-indicator
                 />
        </template> -->
       
    </b-carousel>
</template>

<script>
export default {
    data() {
        return {
            gallery: false,
            al: {
                hasGrayscale: true,
                itemsToShow: 2,
                breakpoints: {
                    768: {
                        hasGrayscale: false,
                        itemsToShow: 4
                    },
                    960: {
                        hasGrayscale: true,
                        itemsToShow: 6
                    }
                }
            },
            items: [
                {
                    title: 'Slide 1',
                    image: 'https://picsum.photos/id/0/1230/500'
                },
                {
                    title: 'Slide 2',
                    image: 'https://picsum.photos/id/1/1230/500'
                },
                {
                    title: 'Slide 3',
                    image: 'https://picsum.photos/id/2/1230/500'
                },
                {
                    title: 'Slide 4',
                    image: 'https://picsum.photos/id/3/1230/500'
                },
                {
                    title: 'Slide 5',
                    image: 'https://picsum.photos/id/4/1230/500'
                },
                {
                    title: 'Slide 6',
                    image: 'https://picsum.photos/id/5/1230/500'
                },
                {
                    title: 'Slide 7',
                    image: 'https://picsum.photos/id/6/1230/500'
                },
                {
                    title: 'Slide 8',
                    image: 'https://picsum.photos/id/7/1230/500'
                }
            ]
        }
    },
    methods: {

    }
}
</script>