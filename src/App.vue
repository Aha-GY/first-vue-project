<template>
  <div>
    <Header />
    <div v-if="isLoading">is loading</div>
    <div v-if="isError">err</div>
    <div v-if="hospitals && hospitals.length">
      <Hospitalcard
        v-for="item in hospitals"
        :key="item.id"
        :address="item.address.woreda"
        :availability="item.availability"
        :photo="item.photo"
        :phoneNumbers="item.phoneNumbers"
        :emails="item.emails"
      />
    </div>
  </div>
</template>

<script>
import Header from '../components/Header';
import Hospitalcard from '@/components/Hospitalcard';
import { useGetHospitadataQuery } from "@/redux/hosApi";

export default {
  components: {
    Header,
    Hospitalcard
  },
  data() {
    return {
      hospitals: [],
      isError: false,
      isLoading: true
    };
  },
  async mounted() {
    try {
      const { data } = await useGetHospitadataQuery();
      this.hospitals = data;
      this.isLoading = false;
    } catch (error) {
      console.error(error);
      this.isError = true;
      this.isLoading = false;
    }
  }
};
</script>
