<template>
    <div class="container">
        <policy-card class="stack" :value="false" policy="LIBERAL"/>
        <span>{{ count }}</span>
    </div>
</template>

<script>
import PolicyCard from '@/ui/cards/policy';

export default {
    components: {
        PolicyCard,
    },

    props: {
        count: Number,
    },
};
</script>

<style module lang="less">
@import "~style";

.stack {
    box-shadow: 0 0 10px gray;
}

.container {
    position: relative;
    
    span {
        position: absolute;
        bottom: 12%;
        width: 100%;
        text-align: center;

        color: white;
        font-size: 36px;
    }
}
</style>
