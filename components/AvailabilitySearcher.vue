<template>
  <v-container :fluid="true" class="pb-10">
    <v-row>
      <v-row class="mr-10">
        <v-col cols="5" class="d-flex justify-end">
          <v-card
            max-width="300"
            max-height="56"
            title="Disponibilidad"
            subtitle="Revisemos tus fechas"
            style="background-color: #228fa2"
          >
          </v-card>
        </v-col>
        <v-col cols="2">
          <DatePicker
            v-model="dateCheckIn"
            style="width: 230px"
            class="flex-grow-0 pr-2"
            labelInput="Check in"
            :min="min"
          />
        </v-col>
        <v-col cols="2">
          <DatePicker
            v-model="dateCheckOut"
            style="width: 230px"
            class="flex-grow-0"
            labelInput="Check out"
          />
        </v-col>
        <v-col cols="3" class="pl-7">
          <v-btn to="/disponibilidad" icon="mdi-calendar-search" />
        </v-col>
      </v-row>
    </v-row>
  </v-container>
</template>

<script lang="ts" setup>
import { DateTime } from 'luxon';

const min = DateTime.local().toString().slice(0, 10);
const dateCheckIn = ref();
const dateCheckOut = ref();
</script>
