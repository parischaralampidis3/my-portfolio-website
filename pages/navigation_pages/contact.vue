<template>
    <div class="container mx-auto  p-12 md:h-screen">       
                <ContactHeader />
                <ContactForm />
                <ContactFooter />
    </div>

</template>

<style scoped>
</style>
 <script>
 import ContactHeader from "~/partial/ContactHeader.vue"
  import ContactForm from "~/partial/ContactForm.vue"
  import ContactFooter from "~/partial/ContactFooter.vue"
    export default{
        name:"contact",
        components:{
    ContactHeader,
    ContactForm,
    ContactFooter
}
    }
</script>