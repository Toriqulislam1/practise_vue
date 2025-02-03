

<script setup>
defineProps({
    msg2: {
    type: String,
    required: true,
  },
  msg3: {
    type: String,
    required: true,
  },

})
</script>


<template>
    <div>
        <h1>Hello, Vue! {{ msg2 }} {{ msg3 }}</h1>
    </div>
</template>

<script>
export default {
    name: 'TestComponent',
    data() {
        return {
            message: 'Welcome to your Vue component!'
        };
    }
};
</script>

<style scoped>
h1 {
    color: #42b983;
}
</style>