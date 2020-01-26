<template>
    <section>
        <table-token-tx-trc21/>
    </section>
</template>

<script>
import TableTokenTxTrc21 from '~/components/TableTokenTxTrc21'

export default {
    components: {
        TableTokenTxTrc21
    },
    head () {
        return {
            title: 'Token TRC21 Transfers'
        }
    },
    async mounted () {
        // Init breadcrumbs data.
        this.$store.commit('breadcrumb/setItems', { name: 'tokentxs-crc21', to: { name: 'tokentxs-crc21' } })
    }
}
</script>

<style scoped>

</style>
