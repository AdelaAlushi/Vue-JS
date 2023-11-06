<template>
  <!-- <h3>Forms created with the Builder pattern in Vue</h3> -->
  <div class="form-container">
    <Form :form-config="formConfig1" />
  </div>
</template>

<script>
import Form from './components/Form.vue';
import './style.css';

export default {
  components: {
    Form,
  },
  data() {
    return {
      formConfig1: [
        // Define the fields for the first form
        // Example:
        {
          type: 'text',
          name: 'username',
          label: 'Username',
          placeholder: 'Enter your email',
        },
        {
          type: 'password',
          name: 'password',
          label: 'Password',
          placeholder: 'Enter your password',
        },
        {
          type: 'text',
          name: 'firstname',
          label: 'First Name',
          placeholder: 'Enter your first name',
        },
        {
          type: 'text',
          name: 'lastname',
          label: 'Last Name',
          placeholder: 'Enter your last name',
        },
        {
          type: 'number',
          name: 'age',
          label: 'Age',
          placeholder: 'Enter your age',
          min: 13,
          max: 65,
          step: 1,
        },
        {
          type: 'tel',
          name: 'phone',
          label: 'Phone',
          placeholder: 'Enter your phone',
        },
        {
          type: 'textarea',
          name: 'address',
          label: 'Address',
          placeholder: 'Enter your address',
        },
      ],
    };
  },
};
</script>
