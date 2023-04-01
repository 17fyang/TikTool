<template>
    <div ref="editor" style="width: 800px; height: 600px;"></div>
  </template>
  
  <script>
    import * as monaco from 'monaco-editor';
  
    export default {
      mounted() {
        const editor = monaco.editor.create(this.$refs.editor, {
          value: 'function hello() {\n\talert("Hello world!");\n}',
          language: 'javascript'
        });
      }
    }
  </script>