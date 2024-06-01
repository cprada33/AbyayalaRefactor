<template>
  <v-container :fluid="true" class="pa-0 pl-15 bg-mygrey">
    <v-row>
      <v-col cols="8">
        <v-row>
          <v-col cols="12" class="d-flex flex-column">
            <div>
              <BookingForm />
            </div>
            <div>
              <BookingPayments />
            </div>
          </v-col>
        </v-row>
      </v-col>
      <v-col cols="4">
        <BookingDetailsBanner />
      </v-col>
    </v-row>
  </v-container>
</template>
