# Custom MCP components - OpenAPI

## OpenAPI

Currently, there is no official OpenAPI specification for the Cortex API, 
but it is rather simple to create an OpenAPI specification for a specific API endpoint, given the integration between the Cortex MCP server infrastructure based on FastMCP and OpenAPI (see https://gofastmcp.com/integrations/openapi#openapi-fastmcp for more details).

To get started, visit the [Cortex API documentation](https://docs-cortex.paloaltonetworks.com/r/Cortex-Cloud-Platform-APIs/Cortex-Cloud-Platform-APIs).
Then proceed with the following steps:
1. Create a yaml file under `/custom_components/openapi` directory with the name of the MCP component, e.g., `custom_cortex_component.yaml`
2. Your custom OpenAPI component should be based on the Cortex API documentation structure for a specific endpoint. Use the builtin files under `/builtin_components/openapi` for reference.
3. After defining the OpenAPI specification, the component is ready to go. The MCP server will collect it automatically.
4. Test the new MCP component by running the MCP server.
