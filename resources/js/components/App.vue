<template>
    <div>
        <h2 class="text-xl font-bold text-center">{{ message }}</h2>
        <file-pond
            name="image"
            ref="pond"
            label-idle="Click to choose image, or drag here ..."
            server="/upload"
        />
    </div>

</template>
<script>
    import vueFilePond from 'vue-filepond';
    import "filepond/dist/filepond.min.css";

    const FilePond = vueFilePond();

    export default {
        components: {
            FilePond
        },
        data() {
            return {
                message: 'Hello, world!'
            }
        }
    }
</script>
