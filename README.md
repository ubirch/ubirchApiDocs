# ubirchApiDocs
ubirch REST API Swagger Docs

If you add a new documentation, add an entry to the file

    ubirchApiDocs/swaggerDocs/docu_paths.json
    
In the following structure:

    {
       "add_swagger_path": false,
       "services": [{
        "name": "<service name>",
        "version": "<version>",
        "uri": "<path to the yaml or json starting under swaggerDocs>"
         }]
     },

Example:

    {
       "add_swagger_path": false,
       "services": [{
           "name": "Ubirch Niomon Service",
           "version": "1.0",
           "uri": "https://niomon.dev.ubirch.com/swagger/swagger.json"
         }]
     },

The add_swagger_path defines, if the Swagger documentation has it's .yaml or .json file
in this project and the path is only a relative one or if the path is a standalone provision of a swagger documentation. 