# Academy Color Encoding System #

This repository contains submodules to the component repositories of the Academy Color Encoding System (ACES). It serves as a convenient way to manage and reference various versions of ACES.

### Versioning

ACES uses [semantic versioning](https://semver.org/). The version number of ACES reflects changes to the [ACES core algorithms](https://github.com/ampas/aces-dev). Additionally, this repository includes a build number that denotes the specific collection of modular components (e.g., [Input and Color Space Transforms](https://github.com/ampas/aces-input-and-colorspaces), [Output Transforms](https://github.com/ampas/aces-output), etc.).

#### Semantic Versioning Structure

- **MAJOR.MINOR.PATCH**: Reflects changes to the core ACES algorithms.
- **Build Number**: Identifies the specific collection of modular components provided by the ACES team, as well as other contributions from the community.

### Modular Components

The modular components of ACES can be updated at any time by the ACES team or by end users. These components do not affect the core functionality of ACES, which is why they are not included in the MAJOR.MINOR.PATCH version number.

### Contributions and Customization

Developers and end users may generate their own modular components. When doing so, they should:

- Create an ACES `transformID` for their components.
- Provide a mechanism for sharing these components with other users (e.g via a CLF referenced in an AMF file).

End users and developers are not required to share their modular components with the community, which allows for extensive customization while preserving the core integrity of the ACES system. For instance, a developer might create custom look transforms or color space conversion transforms for a specific project. While they may choose not to share these with the wider community, they should still create an ACES transformID and CLF files to facilitate sharing these transforms with other vendors involved in the same project.

Note: Sharing custom transforms may necessitate that the software used on the project supports reading CLF and AMF files and can correctly apply these custom transforms within the ACES pipeline.

### Summary

This repository provides a structured and organized way to track and manage different versions of ACES, along with their associated modular components. The build number helps developers reference a specific set of components, while also allowing for the addition of custom components.


## License ##
This project is licensed under the terms of the [LICENSE](./LICENSE.md) agreement.

## Contributing ##
Thank you for your interest in contributing to our project. Before any contributions can be accepted, we require contributors to sign a Contributor License Agreement (CLA) to ensure that the project can freely use your contributions. You can find more details and instructions on how to sign the CLA in the [CONTRIBUTING.md](./CONTRIBUTING.md) file.

## Support ## 
For support, please visit [ACESCentral.com](https://acescentral.com)
