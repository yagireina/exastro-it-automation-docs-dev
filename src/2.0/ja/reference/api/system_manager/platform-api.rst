====================
Exastro Platform API
====================

.. raw:: html

   <div id="swagger-ui"></div>

   <script>
   $(function(){

     $('h1').remove();
     $('#article').attr('id', 'swaggerBody');

     $api_urls = [
       {url: "https://raw.githubusercontent.com/exastro-suite/exastro-platform/1.4/docs/openapi/build/system_manager_reference.yaml", name: "v1.4"},
       {url: "https://raw.githubusercontent.com/exastro-suite/exastro-platform/1.3/docs/openapi/build/system_manager_reference.yaml", name: "v1.3"},
       {url: "https://raw.githubusercontent.com/exastro-suite/exastro-platform/1.2/docs/openapi/build/system_manager_reference.yaml", name: "v1.2"},
       {url: "https://raw.githubusercontent.com/exastro-suite/exastro-platform/1.1/docs/openapi/build/system_manager_reference.yaml", name: "v1.1"},
       {url: "https://raw.githubusercontent.com/exastro-suite/exastro-platform/1.0/docs/openapi/build/system_manager_reference.yaml", name: "v1.0"}
     ];

     // Begin Swagger UI call region
     const ui = SwaggerUIBundle({
       urls: $api_urls,
       dom_id: '#swagger-ui',
       deepLinking: true,
       presets: [
         SwaggerUIBundle.presets.apis,
         SwaggerUIStandalonePreset
       ],
       plugins: [
         SwaggerUIBundle.plugins.DownloadUrl
       ],
       defaultModelsExpandDepth: -1,
       layout: "StandaloneLayout",
     });
     // End Swagger UI call region

     window.ui = ui;
   });
   </script>