<template>
    <div id="example-1">
        <ul v-for="questionList in questionList" :key="questionList.questionList">
            <img :src="questionList.images" style="width: 30%"/>
            <div v-on:click="onClick">
                <button> {{ questionList.choices[0] }} </button>
                <button> {{ questionList.choices[1] }} </button>
                <button> {{ questionList.choices[2] }} </button>
                <button> {{ questionList.choices[3] }} </button>
            </div>
        </ul>
    </div>
</template>

<script>
export default {
    props: {
        questionList: Object
    },
    methods: {
        onClick() {
            if (this.questionList.choices === this.questionList.correctAnswer) {
                console.log("correct");
            } else {
                console.log("false");
            }
        }
    }
}
</script>