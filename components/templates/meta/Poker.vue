<template>
    <v-container>
        <v-row>
            <v-col class="mt-0">
                <MM_Multiple_Input
                    :value = 'data.ref'
                    :action = 'action' 
                    :title = '"Referal link"' 
                    :action_key = '"ref"'
                    />
                <MM_Input
                    :value = 'data.phone'
                    :action = 'action' 
                    :title = '"Phone"' 
                    :action_key = '"phone"'
                    />
                <MM_Multiple_Input_Text 
                    :value = 'data.faq'
                    :action = 'action' 
                    :title = '"Faq"' 
                    :action_key = '"faq"'
                    />
                <MM_Rating 
                    :value = 'data.rating'
                    :action = 'action' 
                    :title = '"Rating"' 
                    :action_key = '"rating"'
                />
                <MM_Input
                    :value = 'data.min_deposit'
                    :action = 'action' 
                    :title = '"Min deposit"' 
                    :action_key = '"min_deposit"'
                    />
                <MM_Input
                    :value = 'data.min_payments'
                    :action = 'action' 
                    :title = '"Min payments"' 
                    :action_key = '"min_payments"'
                    />
                <MM_Input
                    :value = 'data.email'
                    :action = 'action' 
                    :title = '"Email"' 
                    :action_key = '"email"'
                    />
                <MM_Input
                    :value = 'data.year'
                    :action = 'action' 
                    :title = '"Year"' 
                    :action_key = '"year"'
                    />
                <MM_Input
                    :value = 'data.site'
                    :action = 'action' 
                    :title = '"Site"' 
                    :action_key = '"site"'
                    />
                <MM_Input
                    :value = 'data.withdrawal'
                    :action = 'action' 
                    :title = '"Withdrawal"' 
                    :action_key = '"withdrawal"'
                    />
                <MM_Input
                    :value = 'data.rakeback'
                    :action = 'action' 
                    :title = '"Rakeback"' 
                    :action_key = '"rakeback"'
                    />
                <MM_Input
                    :value = 'data.network'
                    :action = 'action' 
                    :title = '"Network"' 
                    :action_key = '"network"'
                    />
                
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
    import MM_Multiple_Input_Text from '../../lib/MM_Multiple_Input_Text'
    import MM_Input from '../../lib/MM_Input'
    import MM_Rating from '../../lib/MM_Rating'
    import MM_Multiple_Input from '../../lib/MM_Multiple_Input'
    export default {
        name: "pokerMeta",
        props: ['data', 'action'],
        components: {MM_Multiple_Input_Text, MM_Input, MM_Rating, MM_Multiple_Input},
        data() {
            return {}
        }
    }
</script>