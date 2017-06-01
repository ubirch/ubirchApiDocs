# ubirchApiDocs
ubirch REST API Swagger Docs

If you add a new documentation, add an entry to the file

    ubirchApiDocs/swaggerDocs/docu_paths.json
    
In the following structure:

      {
        "name": "<service name>",
        "version": "<version>",
        "uri": "<path to the yaml or json starting under swaggerDocs>"
      },

Example:

      {
        "name": "ubirch Key Service",
        "version": "0.5",
        "uri": "/ubirch/key_service/0.5/ubirch_key_service_api.yaml"
      },

The entries have to be a services item of a bundle array:

    {
        "bundlename": "<bundle name>",
        "services": []
    }
