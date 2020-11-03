<template>
    <div>
        <p>WOOF</p>
        <p>{{gorf}}</p>
    </div>
</template>

<script>
import { ref } from "vue"; // <-- Use this line if you're in a Vue 3 app
import testMixin from "@/testmixin"
console.log(testMixin)
export default {
    setup () {
        let gorf = testMixin('dayum')
        return {dog, gorf }
    }
}
function dog(){
    return 'BOOOOOF'
}

</script>

