<script>
export default {
  data() {
    return {
      
    }
  }
}
</script>

<template>
    <div class="container load-more-container">
        <div class="load-more">
            <button>load more</button>
        </div>
    </div>
</template>

<style scoped>
.load-more-container {
    display: flex;
    justify-content: center;
}

.load-more {
    background-color: #0282F9;
    padding: 5px 70px;
    display: inline;
    text-align: center;
}

button {
    background-color: transparent;
    border: 0;
    text-transform: uppercase;
    color: white;
    font-weight: 500;
    font-size: 0.8rem;
}
</style>