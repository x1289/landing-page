<template>
  <div>

    <div id="api-doc-view">
      <h2>API Doc</h2>
      <section>
        <h3>Here is some html...</h3>
        <div class="code-container">
          <pre>
            <code>
      &lt;html&gt;
        &lt;head&gt;
          &lt;title&gt;The page title&lt;/title&gt;
        &lt;/head&gt;
        &lt;body&gt;
          &lt;h1&gt;Hello world!&lt;/h1&gt;
        &lt;/body&gt;
      &lt;/html&gt;</code>
          </pre>
        </div>
      </section>
      <section>
        <h3>And some json...</h3>
        <div class="code-container">
          <pre>
            <code>
      { 
        "title": "Hello world!",
        "lucky_number": 42,
        "numbers": [1, 2, 3]
      }</code>
          </pre>
        </div>
      </section>
    </div>
    <div class="p-3 text-primary-emphasis bg-primary-subtle border border-primary-subtle rounded-3">
      Example element with utilities
    </div>
  </div>
</template>

<style scoped>
#api-doc-view {
  margin: auto;
  max-width: 800px;
}
.code-container {
  max-width: 500px;
  background-color: --bs-primary-bg;
  margin-left: 3rem;
  border-radius: 0.5rem;
  color: white;
}
</style>
