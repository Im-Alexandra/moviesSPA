<template>
    <div class="grid" ref="grid" data-masonry='{ "itemSelector": ".grid-item", "columnWidth": 160 }'>
        <div class="grid-item">
            <img src="https://miro.medium.com/max/3200/1*QBxc5-QaDrLZV9VPHcqG0Q.png">
        </div>
        <div class="grid-item"> <img src="https://mir-s3-cdn-cf.behance.net/project_modules/1400/41fd6377586625.5c8bb65544a31.jpg"></div>
        <div class="grid-item"> <img src="https://miro.medium.com/max/3200/1*QBxc5-QaDrLZV9VPHcqG0Q.png"></div>
        <div class="grid-item"> <img src="https://miro.medium.com/max/3200/1*QBxc5-QaDrLZV9VPHcqG0Q.png"></div>
        <div class="grid-item"> <img src="https://miro.medium.com/max/3200/1*QBxc5-QaDrLZV9VPHcqG0Q.png"></div>
        <div class="grid-item"> <img src="https://miro.medium.com/max/3200/1*QBxc5-QaDrLZV9VPHcqG0Q.png"></div>
        <div class="grid-item"> <img src="https://miro.medium.com/max/3200/1*QBxc5-QaDrLZV9VPHcqG0Q.png"></div>
    </div>
</template>

<script>
//import Masonry from 'masonry-layout';

export default {
    name: 'Overview',
    data(){
        return {
           //msnry: null,
        }
    },
    mounted() {
       /*const { grid } = this.$refs;
        this.msnry = new Masonry(grid, {
            columnWidth: 160,
            itemSelector: '.grid-item',
            percentPosition: true
        });*/
    }
}
</script>

<style>
* { box-sizing: border-box; }

/* ---- grid ---- */

.grid {
  background: #EEE;
}

.grid-item img {
    width: 100%;
    height: auto;
}

/* clearfix */
.grid:after {
  content: '';
  display: block;
  clear: both;
}

/* ---- grid-item ---- */

.grid-item {
padding: 9px;
  width: calc(100% / 4 * 1);
  float: left;
}

.grid-item--width2 { width: 320px; }
.grid-item--width3 { width: 480px; }
.grid-item--width4 { width: 640px; }

.grid-item--height2 { height: 200px; }
.grid-item--height3 { height: 260px; }
.grid-item--height4 { height: 360px; }

</style>