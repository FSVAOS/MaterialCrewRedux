<template>
    <div>
        <v-container fluid grid-list-md>
            <v-layout row wrap fill-height>
                <v-flex md9 xs12>
                    <FlightProgresCard></FlightProgresCard>
                </v-flex>
                <v-flex md3 xs12>
                    <v-img fill-height src="/img/vaos_df_bg-01.svg" gradient="rgba(100,115,201,.33), rgba(25,32,72,.7)">
                        <v-layout pa-2 column align-center fill-height class="lightbox white--text">
                            <v-spacer></v-spacer>
                            <v-avatar size="130">
                                <img src="https://pbs.twimg.com/profile_images/1151671407228706822/UZxOws2b_400x400.jpg" alt="John" style="border: white 3px solid;">
                            </v-avatar>
                            <v-flex shrink style="text-align:center">
                                <div class="headline">Taylor Broad</div>
                                <div class="body-1">BossOfGames | Senior Captain</div>
                            </v-flex>
                        </v-layout>
                    </v-img>
                </v-flex>
            </v-layout>
            <v-layout row wrap>
                <v-flex md9 xs12>
                    <v-card>
                        <v-responsive :aspect-ratio="16/9">
                            <iframe style="height: 100%; width: 100%; border: none;" src="https://simvector.net/"></iframe>
                        </v-responsive>
                    </v-card>
                </v-flex>
                <v-flex md3 xs12>
                    <v-card>
                        <v-img :aspect-ratio="16/9" src="https://i.imgur.com/Fj4dbUx.png" gradient="rgba(30,30,30,0), rgba(30,30,30,.0),rgba(30,30,30,.75)">
                            <v-layout pa-2 column fill-height>
                                <v-spacer></v-spacer>
                                <v-flex shrink style="padding: 0;">
                                    <div class="acf-manufacturer">Daher</div>
                                    <div class="acf-model">TBM-900<span style="float: right">N102TB</span></div>
                                </v-flex>
                            </v-layout>
                        </v-img>
                        <v-list two-line>
                            <v-list-item>
                                <v-list-item-action>
                                    <v-icon>person</v-icon>
                                </v-list-item-action>
                                <v-list-item-content>
                                    <v-list-item-title>Taylor Broad</v-list-item-title>
                                    <v-list-item-subtitle>Owner</v-list-item-subtitle>
                                </v-list-item-content>
                            </v-list-item>
                            <v-list-item>
                                <v-list-item-action>
                                    <v-icon>person</v-icon>
                                </v-list-item-action>
                                <v-list-item-content>
                                    <v-list-item-title>KPDX - Portland International Airport</v-list-item-title>
                                    <v-list-item-subtitle>Current Airport</v-list-item-subtitle>
                                </v-list-item-content>
                            </v-list-item>
                            <v-list-item>
                                <v-list-item-action>
                                    <v-icon>home</v-icon>
                                </v-list-item-action>
                                <v-list-item-content>
                                    <v-list-item-title>KPDX - Portland International Airport</v-list-item-title>
                                    <v-list-item-subtitle>Home Airport</v-list-item-subtitle>
                                </v-list-item-content>
                            </v-list-item>
                            <v-list-item>
                                <v-list-item-action>
                                    <v-icon>access_time</v-icon>
                                </v-list-item-action>
                                <v-list-item-content>
                                    <v-list-item-title>104.5</v-list-item-title>
                                    <v-list-item-subtitle>Hours</v-list-item-subtitle>
                                </v-list-item-content>
                            </v-list-item>
                        </v-list>
                    </v-card>
                </v-flex>
            </v-layout>
        </v-container>
        <!-- Comments and Timeline -->
        <v-container>

        </v-container>
    </div>
</template>

<script>
    import FlightProgresCard from "../../../components/FlightProgressCard";
    export default {
        name: "PostFlight",
        components: {FlightProgresCard},
        props: ['flight']
    }
</script>

<style scoped>
    .acf-manufacturer {
        font-size: 14px;
        line-height: 14px;
    }
    .acf-model {
        font-size: 28px;
        line-height:28px;
    }
</style>
