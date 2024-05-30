<template>
  <v-text-field
    :model-value="modelValue"
    @update:model-value="$emit('update:model-value', $event)"
    variant="outlined"
    :append-inner-icon="icon"
    readonly
    :label="labelInput"
    :hide-details="true"
  >
    <v-menu
      activator="parent"
      :location="location"
      :close-on-content-click="closeOnContentClick"
    >
      <v-date-picker
        :elevation="elevation"
        @update:model-value="date"
        :min="min"
      ></v-date-picker>
    </v-menu>
  </v-text-field>
</template>

<script lang="ts">
import { defineComponent, type PropType } from 'vue';
import { DateTime } from 'luxon';

export default defineComponent({
  name: 'DateInput',
  props: {
    icon: {
      type: String,
      default: 'mdi-calendar-today',
    },
    location: {
      type: String as PropType<'top' | 'bottom'>,
      default: 'bottom',
    },
    elevation: {
      type: String,
      default: '6',
    },
    closeOnContentClick: {
      type: Boolean,
      default: false,
    },
    labelInput: {
      type: String,
      default: 'Escribe aquí',
    },
    modelValue: {
      type: String,
      default: undefined,
    },
    min: {
      type: String,
      default: undefined,
    },
  },
  emits: ['update:model-value'],
  methods: {
    date(value: any) {
      this.$emit('update:model-value', value.toLocaleString().slice(0, 9));
    },
  },
});
</script>
