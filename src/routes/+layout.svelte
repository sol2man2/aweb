<script>
	import '../app.css';
	import { Button, Alert, Card, Navbar, NavBrand, NavLi, NavUl, NavHamburger, Toast } from 'flowbite-svelte';
	import { FireOutline } from 'flowbite-svelte-icons';
</script>

<Navbar let:hidden let:toggle color="primary">
  <NavBrand href="/">
    <img src="/aejalin-ci.png" class="me-3 h-6 sm:h-9" alt="Flowbite Logo" />
    <span class="self-center whitespace-nowrap text-xl font-semibold dark:text-red-800">Aejalin</span>
  </NavBrand>
  <!-- <NavHamburger on:click={toggle} /> -->
  <NavUl {hidden}>
    <NavLi href="/" active={true}>Home</NavLi>
    <NavLi href="/about">About</NavLi>
    <NavLi href="/services">Services</NavLi>
    <NavLi href="/pricing">Pricing</NavLi>
    <NavLi href="/contact">Contact</NavLi>
  </NavUl>
</Navbar>
<slot></slot>
