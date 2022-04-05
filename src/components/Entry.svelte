<script>
  export let data;
  const placeholder = "–";
  let keys = Object.keys(data);

  let key;
  if (data) {
    for (key of keys) {
      if (data[key] == "#N/A") {
        console.log("got it");
        data[key] = "–";
      }
    }
  }
</script>

<!-- {#if data.name != "#N/A" || data.name != "-"} -->
<h1>{data.name}</h1>
<p class="blurb">{data.phrase}</p>
<p class="eyebrow">BIO</p>
<p class="blurb">{data.bio}</p>
<p class="eyebrow">CREATIONS, PASSIONS, PROJECTS, AND ENDEAVORS</p>
<p class="blurb">{data.projects}</p>
<p class="eyebrow">CONTACT</p>
<p class="blurb email">{data.email}</p>
<p class="blurb phone">{data.phone}</p>
<div class="line" />

<!-- {/if} -->
<style>

 
  h1 {
    color: #fa9f4b;
    /* position: absolute; */
    font-family: var(--headline);
    font-style: normal;
    font-weight: 500;
    font-size: 1.33em;
    line-height: 22px;
    margin-bottom: 0.3em;
  }

  .line {
    background-color: #ffffff;
    width: 100%;
    height: 1px;
    margin-top: 4em;
    margin-bottom: 4em;
  }

  .eyebrow {
    font-family: var(--eyebrow);
    font-size: 0.8em;
    margin-bottom: 1em;
  }

  .blurb {
    margin-top: 0;
  }

  .email {
    margin-bottom: 0;
  }

  .phone {
    margin-top: 0;
  }

  p {
    font-family: var(--bodytext);
    font-size: 1em;
  }
</style>
