<script>
  export let title = "SYP Mill Valley";
  export let description = "Description TK";
  export let url = "https://sypartners.com";
  export let keywords = "";
  export let preloadFont = [];
</script>

<svelte:head>
  <title>{title}</title>
  <meta http-equiv="refresh" content="300" />

  <meta name="description" content={description} />
  <meta name="author" content="SYPartners" />
  <meta name="news_keywords" content={keywords} />

  <meta property="og:title" content={title} />
  <meta property="og:site_name" content="SYPartners" />
  <meta property="og:url" content={url} />
  <meta property="og:description" content={description} />
  <meta property="og:type" content="article" />
  <meta property="og:locale" content="en_US" />

  <meta property="og:image" content="{url}/assets/social-facebook.jpg" />
  <meta property="og:image:type" content="image/jpeg" />
  <meta property="og:image:width" content="1200" />
  <meta property="og:image:height" content="600" />

  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:site" content="https://pudding.cool" />
  <meta name="twitter:creator" content="@puddingviz" />
  <meta name="twitter:title" content={title} />
  <meta name="twitter:description" content={description} />
  <meta name="twitter:image:src" content="{url}/assets/social-twitter.jpg" />

  <meta name="robots" content="max-image-preview:large" />

  <link rel="canonical" href="{url}/" />

  {#each preloadFont as href}
    <link rel="preload" {href} as="font" type="font/woff2" crossorigin />
  {/each}
</svelte:head>
