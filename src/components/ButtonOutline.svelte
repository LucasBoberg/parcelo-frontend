<script>
  export let href;
  export let styleName;
</script>

<style>
  a {
    background-color: transparent;
    border-radius: 6rem;
    font-size: 0.9rem;
    line-height: 40px;
    color: #000;
    border: #000 solid 2px;
    text-decoration: none;
    padding: 0.6rem 1.9rem;
    transition: background-color 0.1s ease-in-out;
  }
  a:hover {
    background-color: rgba(0, 0, 0, 0.1);
  }
</style>

<a {href} class={styleName}><slot/></a>