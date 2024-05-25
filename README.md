# Quick Open Tool for LabVIEW Developers

## Overview

Welcome to Quick Open, a tool designed to streamline your LabVIEW development process by allowing you to open any VI quickly and efficiently. Inspired by the "Quick Open" feature in Visual Studio Code, this tool aims to enhance your productivity by reducing the time spent navigating through LabVIEW projects.

### Future Implementation

The current implementation serves as a proof of concept. The final version of Quick Open will include:

- **LabVIEW Menu Integration:** Quick Open will be accessible from a dedicated menu item within LabVIEW.
- **Custom Shortcut Assignment:** Users will be able to assign a custom keyboard shortcut to invoke Quick Open, similar to how Quick Drop is accessed.
- **Include more files in searchable list:** In this proof of concept version, it will open all VIs in the memory, it can be enchanced to open any VIs from the opened LabVIEW project.

## Features

- **Quick Access:** Open any VI in your project swiftly using a search-based approach.
- **Faster Search** It supports a search pattern similar to fuzzy matching. It finds matches even for misspelled or partially typed words similar to VS Code Quick Open feature.  
- **Easy Integration:** Currently leverages LabVIEW's Quick Drop functionality to invoke the Quick Open UI.
- **User-Friendly Interface:** A clean and intuitive UI that allows you to find and open VIs with minimal effort.

## Installation

1. **Download the Files:**
   - Download the `Quick Open as QuickDrop Plugin.vi` and `QuickOpen.vi` files from the repository.

2. **Copy to Quick Drop Plugin Location:**
   - Navigate to your LabVIEW Quick Drop plugin directory. This is typically located at:
     ```
     <LabVIEW>\resource\dialog\QuickDrop\plugins\
     ```
   - Copy the downloaded `Quick Open as QuickDrop Plugin.vi` and `QuickOpen.vi` files into this directory.
   - Refer the link for more details and other options - [How to install a Quick Drop Keyboard Shortcut plugin](https://forums.ni.com/t5/Quick-Drop-Enthusiasts/How-to-install-a-Quick-Drop-Keyboard-Shortcut-plugin/m-p/3896383)

## Usage

### Invoking Quick Open

Currently, Quick Open is integrated with LabVIEW's Quick Drop plugin as a temporary solution. Follow these steps to use it:

1. **Open Quick Drop:**
   - Press `Ctrl + Space` to open the Quick Drop window in LabVIEW.

2. **Invoke Quick Open:**
   - In the Quick Drop window, type the command `Ctrl + A` for Quick Open.
   - For now `Ctrl + A` is assigned as a default, which can be modifed in Quick Drop window.

3. **Search and Open VI:**
   - Start typing the name of the VI you want to open.
   - Select the desired VI from the search results using up and down arrows
   - Press `Enter` to open the selected VI.

## Contributing

We welcome contributions from the community to enhance Quick Open. To contribute:

1. **Fork the Repository:**
   - Click the "Fork" button on the GitHub repository page.

2. **Create a Branch:**
   - Create a new branch for your feature or bugfix.
   ```bash
   git checkout -b feature/YourFeatureName
   ```

 3. **Commit Your Changes:***
    - Make your changes and commit them with a descriptive message.
     ```bash
     git commit -m "Add feature: YourFeatureName"
     ```

4. **Push to Your Branch:**
   - Push your changes to your forked repository.
   ```bash
   git push origin feature/YourFeatureName
   ```
5. **Create a Pull Request:**
   - Open a pull request on the original repository and describe your changes in detail.
