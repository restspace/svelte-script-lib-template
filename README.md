# Svelte + TS + Vite > class library

This is a variation of the standard npm install vite TS/Svelte library. Its build output is a js file which can be loaded as a script on a webpage and then used in code on the page as a class e.g.

    <body>
      <div id="container"></div>
      <script type="module">
        import { SvelteComponent } from "https://myfiles.com/path/to/svelteComponent.js";

        const x = new SvelteComponent({
          target: document.getElementById("container"),
          props: {
            prop1: prop1val
          }
        });
      </script>
    </body>