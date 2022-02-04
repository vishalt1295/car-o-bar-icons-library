<template>
  <Navbar />
  <div class="container mt-3">
    <div class="row mb-4">
      <h4 class="mb-4 mt-2">Usage</h4>
      <div class="col-md-6">
        <div class="icon-demo d-flex justify-content-evenly">
          
          <i class="cobi-house-duotone"></i>

          <i class="cobi-house-fill"></i>

          <i class="cobi-house-outline"></i>

        </div>
        <div class="highlight">
          <ul class="list-unstyled usage">
            <li>
              <pre
                tabindex="0"
                class="chroma"
              ><code class="language-html" data-lang="html"><span class="p">&lt;</span><span class="nt">i</span> <span class="na">class</span><span class="o">=</span><span class="s">&#34;cobi-house-duotone&#34;</span><span class="p">&gt;&lt;/</span><span class="nt">i</span><span class="p">&gt;</span></code>
          </pre>
            </li>

            <li>
              <pre
                tabindex="0"
                class="chroma"
              ><code class="language-html" data-lang="html"><span class="p">&lt;</span><span class="nt">i</span> <span class="na">class</span><span class="o">=</span><span class="s">&#34;cobi-house-fill&#34;</span><span class="p">&gt;&lt;/</span><span class="nt">i</span><span class="p">&gt;</span></code>
          </pre>
            </li>

            <li>
              <pre
                tabindex="0"
                class="chroma"
              ><code class="language-html" data-lang="html"><span class="p">&lt;</span><span class="nt">i</span> <span class="na">class</span><span class="o">=</span><span class="s">&#34;cobi-house-outline&#34;</span><span class="p">&gt;&lt;/</span><span class="nt">i</span><span class="p">&gt;</span></code>
          </pre>
            </li>
          </ul>
        </div>
      </div>
    </div>

    <Icons />

  </div>
</template>

<script>
import Navbar from "./Navbar.vue";
import Icons from './Icons.vue';

export default {
  components: { Navbar, Icons },
};
</script>

<style scoped>
.icon-demo {
  padding: 1.25rem;
  border: 1px solid rgba(0, 0, 0, 0.1);
  border-top-left-radius: 0.25rem;
  border-top-right-radius: 0.25rem;
}

.highlight {
  padding: 1.25rem;
  /*margin-bottom: 1.5rem;*/
  background-color: #f8f9fa;
  border-radius: 0 0 0.25rem 0.25rem;
  /*border-radius: 0.25rem;*/
}

pre {
  margin-top: revert;
}

.chroma .nt {
  color: #2f6f9f;
}

.chroma .na {
  color: #006ee0;
}

.chroma .o {
  color: #555;
}

.chroma .s {
  color: #d73038;
}

.usage {
  padding-top: 1rem !important;
}

.icon-demo img {
  width: 3rem;
}
.icon-library img {
  width: 3rem;
}
</style>
