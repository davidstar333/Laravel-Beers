<template>
    <div class="container">
        <div class="row justify-content-center">
            <div class="col-md-12">
                <div class="card">
                    <div class="card-header">
                        <button id="brew_btn" class="btn btn-primary pull-left">Brew</button>
                    </div>
                    <div class="card-body">
                        <TankComponent v-for="(tank, i) in tanks"
                        :key="i"
                        :amount="tank.amount"
                        :tank_name="tank.tank_name"
                        />
                    </div>
                    <div class="card-footer">
                        <button id="move_btn" class="btn btn-success">Move</button>
                        <button id="dump_btn" class="btn btn-secondary">Dump</button>
                        <button id="keg_btn" class="btn btn-custom">Keg</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import TankComponent from './TankComponent.vue'

export default {
    name: 'Main',
    components: {
        TankComponent,
    },
    mounted() {
        console.log('Component mounted.')
    },
    data() {
        return {
            tanks: [
                {
                    amount: 5,
                    tank_name: 'Tank1'
                },
                {
                    amount: 10,
                    tank_name: 'Tank2'
                },
                {
                    amount: 13,
                    tank_name: 'Tank3'
                },
                {
                    amount: 14,
                    tank_name: 'Tank4'
                },
                {
                    amount: 19,
                    tank_name: 'Tank5'
                }
            ]
        }
    }
}
</script>
