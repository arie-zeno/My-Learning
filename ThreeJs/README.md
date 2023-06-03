# Three JS
Three JS Merupakan framework webGl (javascript)

- ### Struktur Program
  - Buat file html dan js untuk mengimport ThreeJs
    - File HTML
      ```HTML
          <!DOCTYPE html>
          <html lang="en">
              <head>
                  <meta charset="utf-8">
                  <title>My first three.js app</title>
                  <style>
                      body { margin: 0; }
                  </style>
              </head>
              <body>
                  <script type="module" src="/main.js"></script>
              </body>
          </html>
      ```

    - main.js
        ```javascript
        import * as THREE from 'three';
        ```
            nama file bebas

  
  - Sisipkan code berikut kedalam tag `<head> </head>`
     ```javascript
      <script async src="https://unpkg.com/es-module-shims@1.6.3/dist/es-module-shims.js"></script>

      <script type="importmap">
        {
          "imports": {
            "three": "https://unpkg.com/three@<version>/build/three.module.js",
            "three/addons/": "https://unpkg.com/three@<version>/examples/jsm/"
          }
        }
      </script>
      ```
      Ganti `<version>` dengan versi ThreeJs yang akan digunakan.
- ### Membuat Scene
  