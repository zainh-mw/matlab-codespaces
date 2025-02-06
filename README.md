# Run MATLAB in GitHub Codespaces

This repository shows how to run MATLAB&reg; in [GitHub&trade; Codespaces](https://github.com/features/codespaces), so you can quickly start a development environment for developing the MATLAB code hosted in your Github repository.


## Table of Contents
- [When Should I Use Codespaces for MATLAB?](#when-should-i-use-codespaces-for-matlab)
- [Choose a Configuration](#choose-a-configuration)
- [Use MATLAB in Codespaces](#use-matlab-in-codespaces)
  - [What Can I Do With MATLAB in VS Code?](#what-can-i-do-with-matlab-in-vs-code)
  - [What Can I Do With MATLAB in JupyterLab?](#what-can-i-do-with-matlab-in-jupyterlab)
- [Related Links](#related-links)    


## When Should I Use Codespaces for MATLAB?

A [codespace (GitHub Docs)](https://docs.github.com/en/codespaces/overview) is a development environment you can run in the cloud. If you own a Github repository hosting MATLAB Code, a codespace allows users of your repository to:
- Configure a consistent and customizable development environment.
- Run your MATLAB code with any other software.
- Use Git to contribute back to your repository.

## Choose a Configuration

Codespaces run in Docker containers called development containers, or [dev containers (GitHub Docs)](https://docs.github.com/en/codespaces/setting-up-your-project-for-codespaces/adding-a-dev-container-configuration/introduction-to-dev-containers). You can customize how MATLAB is installed in your codespace by modifying the configuration file of the dev container, named `devcontainer.json`. Choose the configuration that corresponds to your desired use case.

| Use Case  | Recommendation | Start Codespace Using Recommended Configuration |
| ------------- | ------------- |------------- |
|Use MATLAB only|Use a prebuilt [MATLAB Container on Docker Hub](https://hub.docker.com/r/mathworks/matlab). Configure your codespace using [devcontainer.json](.devcontainer/devcontainer.json).|[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new/mathworks-ref-arch/matlab-codespaces?template=false&devcontainer_path=.devcontainer%2Fdevcontainer.json)|
|Tailor MATLAB installation with specific toolboxes or other software|Create a custom MATLAB container image using [MATLAB Dockerfile](https://github.com/mathworks-ref-arch/matlab-dockerfile). You can see an example Dockerfile in the `.devcontainer/using-matlab-dockerfile` folder. Configure your codespace using [devcontainer.json](.devcontainer/using-matlab-dockerfile/devcontainer.json).|[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new/mathworks-ref-arch/matlab-codespaces?template=false&devcontainer_path=.devcontainer%2Fusing-matlab-dockerfile%2Fdevcontainer.json)|
|Add MATLAB to an existing devcontainer configuration|Use the [MATLAB Feature for Devcontainers](https://github.com/mathworks/devcontainer-features/tree/main/src/matlab). Configure your codespace using [devcontainer.json](.devcontainer/using-devcontainer-feature/devcontainer.json)|[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new/mathworks-ref-arch/matlab-codespaces?template=false&devcontainer_path=.devcontainer%2Fusing-devcontainer-feature%2Fdevcontainer.json)||

## Use MATLAB in Codespaces 

Use your MATLAB codespace to:
- Run & Debug `.m` files in VS Code
- Run MATLAB code in Jupyter Notebooks in both VS Code and JupyterLab
- Switch to the MATLAB IDE to use more MATLAB features.

By default, your MATLAB codespace starts in a [Visual Studio Code](https://code.visualstudio.com/) environment, and MATLAB opens in a browser tab.

![VSCode In Codespaces](img/VSCodeInCodespaces.png)

For details on using MATLAB in VS Code in your codespace, see [What Can I Do With MATLAB in VS Code?](#what-can-i-do-with-matlab-in-vs-code)

For details on using MATLAB in JupyterLab in your codespace, see [What Can I Do With MATLAB in JupyterLab?](#what-can-i-do-with-matlab-in-jupyterlab)




### What Can I Do With MATLAB in VS Code?

Once you have MATLAB set up in your codespace, you can use VS Code to: 

1. **Run & Debug MATLAB files in the VS Code editor.**</br>
   
   ![Run and Debug MATLAB in VS Code](img/RunAndDebugInVSCode.gif)
   
   For more information, see [MATLAB Extension for Visual Studio Code](https://github.com/mathworks/MATLAB-extension-for-vscode).


2. **Access the MATLAB IDE in a browser tab.**</br>

   ![MATLAB Proxy](img/MATLABinBrowser.png)

   For more information on using MATLAB in the browser, see [MATLAB Proxy](https://github.com/mathworks/matlab-proxy).

3. **Run MATLAB code using Jupyter Notebooks.**</br>
   
   ![Jupyter Notebook In VS Code](img/JupyterNotebookInVSCode.gif)

   For more information on using Jupyter Notebooks in VS Code, see [Jupyter Notebooks in VS Code](https://code.visualstudio.com/docs/datascience/jupyter-notebooks)

### What Can I Do With MATLAB in JupyterLab?

To use MATLAB in JupyterLab in your codespace:

1. Set up JupyterLab by following the steps in [Open Your Codespace in JupyterLab (Github)](https://docs.github.com/en/codespaces/developing-in-a-codespace/getting-started-with-github-codespaces-for-machine-learning#opening-your-codespace-in-jupyterlab).

  ![Open In JupyterLab](img/OpenInJupyterLab.gif)
  
2. Install the [MATLAB Integration for Jupyter](https://github.com/mathworks/jupyter-matlab-proxy) in your codespace.

After setting up and MATLAB and JupyterLab in your codespace, you can:

1. **Run MATLAB code using Jupyter Notebooks.**</br>
   
   ![Run MATLAB code using Jupyter Notebooks](https://github.com/mathworks/jupyter-matlab-proxy/raw/main/img/JupyterKernel.gif)

2. **Access the MATLAB in a browser window.**</br>
      
   ![Access the MATLAB in a browser window](https://github.com/mathworks/jupyter-matlab-proxy/raw/main/img/JupyterMATLABDesktop.gif)


## Related Links

- [Overview of Codespaces (GitHub)](https://docs.github.com/en/codespaces/overview)
- [Development Container Features (GitHub)](https://github.com/devcontainers/features/)
- [Development Container Specification (Microsoft&reg;)](https://containers.dev/implementors/spec/)
- [Setting Your Default Editor for Codespaces (GitHub)](https://docs.github.com/en/codespaces/setting-your-user-preferences/setting-your-default-editor-for-github-codespaces)
- [Run Dev Containers in VS Code (VS Code Docs) ](https://code.visualstudio.com/docs/devcontainers/create-dev-container)

---

Copyright 2024 The MathWorks, Inc.

---
