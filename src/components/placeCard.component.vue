<template>
<div class='flex-auto flex justify-between items-center pt2 pb2 pl1 pr2 b fw4 gray bb b--light-gray'>
    <div>{{ placeLabel }}</div>
    <div class='flex flex-column tr'>
        <span>{{ hotelsFound }}</span>
        <span>Hotels</span>
    </div>
</div>
</template>

<script>

export default {
    name: 'placeCard',
    props: {
        /* 
            @placeData main data of thaty place
            @placeLabel string to display the main label
            @hotelFound for of hotels
        */ 

        placeData: {
            type: Object,
            default: () => {}
        },

        placeLabel: {
            type: String,
            default: ""
        },

        hotelsFound: {
            type: Number,
            default: "0"
        }

    },
}
</script>
