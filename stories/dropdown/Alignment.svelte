<script lang="ts">
  import {
    Dropdown,
    DropdownItem,
    DropdownMenu,
    DropdownToggle
  } from 'sveltestrap';

  let isOpen = false;
</script>

<Dropdown {isOpen} toggle={() => (isOpen = !isOpen)}>
  <DropdownToggle caret>Dropdown's menu is right-aligned</DropdownToggle>
  <DropdownMenu right>
    <DropdownItem header>Header</DropdownItem>
    <DropdownItem disabled>Action</DropdownItem>
    <DropdownItem>Another Action</DropdownItem>
  </DropdownMenu>
</Dropdown>
