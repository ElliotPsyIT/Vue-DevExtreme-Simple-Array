<template>
  <div class="card">
    <dx-grid
      :rows="rows"
      :columns="columns"
    >
      <dx-table />
      <dx-table-header-row />
    </dx-grid>
  </div>
</template>

<script>
import "@devexpress/dx-vue-grid-bootstrap4/dist/dx-vue-grid-bootstrap4.css";
import {
  DxGrid,
  DxTable,
  DxTableHeaderRow,
} from '@devexpress/dx-vue-grid-bootstrap4';

export default {
  name: "App",
  data() {
    return {
      columns: [
        { name: "name", title: "Name" },
        { name: "sex", title: "Sex" },
        { name: "city", title: "City" },
        { name: "car", title: "Car" }
      ],
      rows: [
        { sex: "Female", name: "Sandra", city: "Las Vegas", car: "Audi A4" },
        { sex: "Male", name: "Paul", city: "Paris", car: "Nissan Altima" },
        { sex: "Male", name: "Mark", city: "Paris", car: "Honda Accord" },
        { sex: "Male", name: "Paul", city: "Paris", car: "Nissan Altima" },
        { sex: "Female", name: "Linda", city: "Austin", car: "Toyota Corolla" },
        {
          sex: "Male",
          name: "Robert",
          city: "Las Vegas",
          car: "Chevrolet Cruze"
        },
        { sex: "Female", name: "Lisa", city: "London", car: "BMW 750" },
        { sex: "Male", name: "Mark", city: "Chicago", car: "Toyota Corolla" },
        {
          sex: "Male",
          name: "Thomas",
          city: "Rio de Janeiro",
          car: "Honda Accord"
        },
        { sex: "Male", name: "Robert", city: "Las Vegas", car: "Honda Civic" },
        { sex: "Female", name: "Betty", city: "Paris", car: "Honda Civic" },
        {
          sex: "Male",
          name: "Robert",
          city: "Los Angeles",
          car: "Honda Accord"
        },
        {
          sex: "Male",
          name: "William",
          city: "Los Angeles",
          car: "Honda Civic"
        },
        { sex: "Male", name: "Mark", city: "Austin", car: "Nissan Altima" }
      ]
    };
  },
  components: {
    DxGrid,
    DxTable,
    DxTableHeaderRow,
  }
};
</script>

<style></style>
