<template>
    <div class="container">
        <div class="row">
            <div class="col-xs-12">
                <br>
                <button class="btn btn-primary" @click="selectedComponent = 'appBlue'">Load Blue Template</button>
                <button class="btn btn-success" @click="selectedComponent = 'appGreen'">Load Green Template</button>
                <button class="btn btn-danger" @click="selectedComponent = 'appRed'">Load Red Template</button>
                <hr>
                <component :is="selectedComponent">
                    <p>
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam tempus eget nisl nec posuere. Proin suscipit augue quis purus aliquet porttitor. Curabitur gravida vulputate tellus, sit amet fringilla enim tincidunt at. Sed arcu purus, lacinia a quam at, dictum viverra est. Ut non accumsan nisi. Nullam faucibus, nunc et venenatis sollicitudin, lectus ligula semper tellus, quis dignissim turpis nisi sed elit. Pellentesque faucibus nisl ut velit egestas, ut semper velit iaculis. Etiam auctor cursus hendrerit. Suspendisse malesuada tincidunt venenatis. Duis suscipit luctus metus, id porta lacus hendrerit quis. Fusce nunc justo, aliquet eleifend nisi ut, pellentesque bibendum risus.
                    </p>
                </component>
            </div>
        </div>
    </div>
</template>

<script>
    import Blue from './components/Blue.vue';
    import Green from './components/Green.vue';
    import Red from './components/Red.vue';

    export default {
        components: {
            appBlue: Blue,
            appGreen: Green,
            appRed: Red
        },
        data: function() {
            return {
                selectedComponent: ''
            };
        }
    }
</script>

<style>
</style>
