<script setup>
import GuestLayout from '@/Layouts/GuestLayout.vue';
import Label from '@/Components/InputLabel.vue';
import TextInput from '@/Components/TextInput.vue';

const emitTest = e => console.log(e);
</script>

<template>
<GuestLayout>
    <Label>タイトル</Label>
    <TextInput
    modelValue="初期値"
    @update:model-value="emitTest"></TextInput>
</GuestLayout>
</template>
