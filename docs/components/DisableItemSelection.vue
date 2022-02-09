<template>
  <treeselect :multiple="false" :options="options" :value="value" />
</template>

<script>
/* eslint-disable */
export default {
  data: () => ({
    options: [
      {
        id: "folder",
        label: "Normal Folder",
        children: [
          {
            id: "disabled-checked",
            label: "Checked",
            isDisabled: true,
          },
          {
            id: "disabled-unchecked",
            label: "Unchecked",
            isDisabled: true,
          },
          {
            id: "item-1",
            label: "Item",
          },
        ],
      },
      {
        id: "disabled-folder",
        label: "Disabled Folder",
        isDisabled: true,
        children: [
          {
            id: "item-2",
            label: "Item",
          },
          {
            id: "item-3",
            label: "Item",
          },
        ],
      },

      {
        id: "disabled-folder-3",
        label: "Disabled Folder",
        disabled: true,
        children: [
          {
            id: "item-22",
            label: "Item",
          },
          {
            id: "item-33",
            label: "Item",
          },
        ],
      },

      {
        id: "disabled-folder-4",
        label: "Disabled Folder",
        children: [
          {
            id: "item-44",
            label: "Item",
            disabled: true,
          },
          {
            id: "item-55",
            label: "Item",
          },
        ],
      },
    ],
    value: "disabled-checked",
  }),
};
</script>
