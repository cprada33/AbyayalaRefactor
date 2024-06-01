<template>
  <v-container :fluid="true">
    <v-row style="height: 80px">
      <v-row class="mr-10">
        <v-col cols="5" class="d-flex justify-end">
          <v-sheet
            class="bg-second rounded text-center"
            style="max-height: 58px"
          >
            <v-container class="h-50">
              <v-row class="h-50 my-n5 color-white" style="font-weight: 700">
                <v-col cols="12">DISPONIBILIDAD</v-col>
              </v-row>
              <v-row class="h-50 mt-10 color-white">
                <v-col cols="12">Veamos tus fechas</v-col>
              </v-row>
            </v-container>
          </v-sheet>
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
          <v-btn
            class="bg-second color-white"
            to="/disponibilidad"
            icon="mdi-calendar-search"
          />
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
