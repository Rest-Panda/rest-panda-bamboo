# rest-panda-bambu
Banbu is a REST Panda project extensions support

## REST Panda extension (BAMBU)
bambu {
    # BAMBU Name
    name = "example",

    # BAMBU base path
    basePath = "/example",

    # MBAMBU MODEL
    model = [
        {
            type = "ObjectExample",
            fields = [
                {
                    type = "String",
                    name = "Name",
                    description = "Example name"
                }
            ]
        }
    ],
    # BAMBU API
    api = [
        # GET All Example
        {
            path = "/",
            method = "GET",
            description = "Get all example",
            queryParams = param1|param2|param3,
            outputRef = "LIST/#ObjectExample"
        },
        # GET by ID Example
        {
            path = "/{id}",
            method = "GET",
            description = "Get by id example",
            outputRef = "#ObjectExample"
        },
        # PUT Example
        {
            path = "/",
            method = "PUT",
            description = "Update example",
            inputRef = "#ObjectExample",
            outputRef = "#ObjectExample"
        },
        # POST Example
        {
            path = "/",
            method = "POST",
            description = "Create example",
            inputRef = "#ObjectExample",
            outputRef = "#ObjectExample"
        },
         # DELETE all Example
        {
            path = "/",
            method = "DELETE",
            description = "Deleta all example"

        }
    ]}
