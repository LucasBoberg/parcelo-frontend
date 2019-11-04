<script>
  export let href;
  export let styleName;
  export let primary = false;
</script>

<style>
  a {
    background-color: #000;
    border-radius: 6rem;
    font-size: 0.9rem;
    line-height: 40px;
    color: #FFF;
    cursor: pointer;
    border: #000 solid 2px;
    text-decoration: none;
    padding: 0.6rem 1.9rem;
    transition: background-color 0.1s ease-in-out;
  }
  a:hover {
    background-color: rgba(0, 0, 0, 0.9);
  }
  .primary {
    background-color: #32E37F;
    border: #32E37F solid 2px;
  }
  .primary:hover {
    background-color: rgba(50, 227, 127, 0.8);
  }
</style>

<a {href} class:primary class={styleName}><slot/></a>