<template>
  <div>
    <div v-for="(phoneNumber, index) in addedPhoneNumbers" :key="index">
      <input v-model="addedPhoneNumbers[index]" class="cc-input" />
    </div>
    <button class="blue-button font-semibold" @click="addPhoneNumberInput">
      + Add number
    </button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      addedPhoneNumbers: [],
    };
  },
  methods: {
    addPhoneNumberInput() {
      this.addedPhoneNumbers.push(''); // Add a new input field with an empty value
    },
  },
};
</script>

<style scoped>
.blue-button {
  color: #4a8ae7;
  font-size: 0.7em;
  background-color: transparent;
  border: none;
  cursor: pointer;
}
.cc-input {
  padding: 17px 16px;
  margin-top: 14px;
  border-radius: 4px;
  border: 2px solid #d2d0d0b4;
  font-size: 16px;
}
</style>
