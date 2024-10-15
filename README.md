# Scanspire API Documentation

This repository hosts the Swagger UI for Scanspire's API documentation. It uses GitHub Pages to provide a beautiful, interactive interface for exploring and understanding the Scanspire API.

## Viewing the Documentation

You can view the live API documentation at [[https://asimd.github.io/scanspire-apidocs]([https://apidocs.scanspire.com](https://apidocs.scanspire.com/)/)](https://asimd.github.io/scanspire-apidocs).

## API Specification

The API specification is defined in the `swagger.yaml` file in the root of this repository. This file is dynamically loaded by Swagger UI to generate the interactive documentation.

## Structure

The repository is structured as follows:

- `index.html`: The main HTML file that loads Swagger UI.
- `swagger.yaml`: The main OpenAPI/Swagger specification file.
- `auth_controller.yaml`: Specification for authentication endpoints.
- `scan_controller.yaml`: Specification for scan-related endpoints.
- `domain_controller.yaml`: Specification for domain-related endpoints.
- `dist/`: Directory containing the Swagger UI assets.

## Updating the Documentation

To update the API documentation:

1. Modify the relevant YAML files (`swagger.yaml`, `auth_controller.yaml`, `scan_controller.yaml`, or `domain_controller.yaml`).
2. Commit and push your changes to the `master` branch.
3. GitHub Pages will automatically rebuild and deploy the updated documentation.

## Local Development

To run the documentation locally:

1. Clone this repository:
   ```
   git clone https://github.com/asimd/scanspire-apidocs.git
   cd scanspire-apidocs
   ```

2. Serve the directory with a local HTTP server. For example, using Python:
   ```
   python -m http.server 8000
   ```

3. Open your browser and navigate to `http://localhost:8000`.

## Automatic Updates

This repository is set up with a GitHub Actions workflow that periodically checks for updates to Swagger UI. When updates are available, it will automatically create a pull request to update the dependency.

## Contributing

If you find any issues or have suggestions for improving the API documentation, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

This API documentation is powered by [Swagger UI](https://github.com/swagger-api/swagger-ui) and hosted with GitHub Pages.
