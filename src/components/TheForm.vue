<script setup>
    import { ref } from 'vue'

    const fname = ref('')
    const lname = ref('')
    const email = ref('')
    const purpose = ref('')
    const briefs = ref('')
</script>

<template>
  <!--Brief-->
  <section class="brief">
        <div>
            <h1>Give Us a Brief</h1>
            <form @submit.prevent="brief">
                <div>
                    <label for="fname">First Name</label>
                    <input v-model="fname" type="text" placeholder="Richard">
    
                    <label for="lname">Last Name</label>
                    <input v-model="lname" type="text" placeholder="Smith">
                    
                    <label for="email">Email</label>
                    <input v-model="email" type="email" placeholder="richardsmith@email.com">
                </div>
                
                <div>
                    <label for="select">Select what suits you</label><br>
                    <select v-model="purpose">
                        <option value="Scoial Media">Social Media</option>
                        <option value="Online Ads">Online Ads</option>
                        <option value="other">Other</option>
                    </select>
                </div>

                <div class="brieftext">
                    <label for="brief">What are you looking for ?</label><br>
                <textarea v-model="briefs" placeholder="your message"></textarea>
                </div>
            </form>
        </div>
    </section>
</template>

<style scoped>
</style>
