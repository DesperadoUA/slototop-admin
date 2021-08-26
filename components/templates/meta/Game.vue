<template>
    <v-container>
        <v-row>
            <v-col class="mt-0">
                <MM_Image 
                    :value = 'data.banner' 
                    :title = '"Banner"'
                    :action = 'action'
                    :action_key = '"banner"' 
                />
                <MM_Input
                    :value = 'data.jackpot'
                    :action = 'action' 
                    :title = '"Jackpot"' 
                    :action_key = '"jackpot"'
                />
                <MM_Input
                    :value = 'data.risk_game'
                    :action = 'action' 
                    :title = '"Risk game"' 
                    :action_key = '"risk_game"'
                />
                <MM_Input
                    :value = 'data.max_gain'
                    :action = 'action' 
                    :title = '"Max gain"' 
                    :action_key = '"max_gain"'
                />
                <MM_Input
                    :value = 'data.max_bet'
                    :action = 'action' 
                    :title = '"Max bet"' 
                    :action_key = '"max_bet"'
                />
                <MM_Input
                    :value = 'data.min_bet'
                    :action = 'action' 
                    :title = '"Min bet"' 
                    :action_key = '"min_bet"'
                />
                <MM_Input
                    :value = 'data.iframe'
                    :action = 'action' 
                    :title = '"iframe"' 
                    :action_key = '"iframe"'
                />
                <MM_Multiple_Two_Input
                    :value = 'data.details'
                    :action = 'action' 
                    :title = '"Details"' 
                    :action_key = '"details"'
                    />             
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
    /* TO DO: characters component */
    import MM_Multiple_Input_Text from '../../lib/MM_Multiple_Input_Text'
    import MM_Input from '../../lib/MM_Input'
    import MM_Multiple_Input from '../../lib/MM_Multiple_Input'
    import MM_Checkbox from '../../lib/MM_Checkbox'
    
    export default {
        name: "slotMeta",
        props: ['data', 'action'],
        components: {MM_Multiple_Input_Text, MM_Input, MM_Multiple_Input, MM_Checkbox},
        data() {
            return {}
        },
        mounted(){
            console.log(this.data)
        }
    }
</script>