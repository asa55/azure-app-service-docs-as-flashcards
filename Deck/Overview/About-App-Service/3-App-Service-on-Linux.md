##

App Service can also host web apps natively on Linux for supported application stacks. It can also run custom Linux `_____` (also known as Web App for **Containers**).

%

App Service can also host web apps natively on Linux for supported application stacks. It can also run custom Linux **containers** (also known as Web App for **Containers**).

##

App Service on Linux supports a number of language specific built-in

%

images

##

With App Service, just deploy your code. Supported languages include:

- `_____`
- `_____`
- `_____`
- `_____`
- `_____`
- `_____`
- `_____`

%

- Node.js
- Java (8, 11, and 17)
- Tomcat
- PHP
- Python
- .NET Core
- Ruby

##

For App Service on Linux, run the following Azure CLI command to view the latest languages and supported versions:

%

`az webapp list-runtimes --os linux `

##

For App Service, if the runtime your application requires is not supported in the built-in images, you can deploy it with a custom

%

container

##

Outdated runtimes are periodically removed from the Web Apps Create and Configuration blades in the Portal. These runtimes are hidden from the Portal when they are deprecated by the maintaining organization or found to have significant vulnerabilities. These options are hidden to guide customers to the `_____` runtimes where they will be the most successful.

%

Outdated runtimes are periodically removed from the Web Apps Create and Configuration blades in the Portal. These runtimes are hidden from the Portal when they are deprecated by the maintaining organization or found to have significant vulnerabilities. These options are hidden to guide customers to the **latest** runtimes where they will be the most successful.

##

When an outdated runtime is hidden from the Portal, any of your existing sites using that version will continue to `_____`. If a runtime is fully removed from the App Service platform, your Azure subscription owner(s) will receive an email notice before the removal.

%

When an outdated runtime is hidden from the Portal, any of your existing sites using that version will continue to **run**. If a runtime is fully removed from the App Service platform, your Azure subscription owner(s) will receive an email notice before the removal.

##

If you need to create another web app with an outdated runtime version that is no longer shown on the Portal see the language configuration guides for instructions on how to get the runtime version of your site. You can use the Azure CLI to create another site with the same runtime. Alternatively, you can use the Export `_____` button on the web app blade in the Portal to export an ARM `_____` of the site. You can reuse this `_____` to deploy a new site with the same runtime and configuration.

%

If you need to create another web app with an outdated runtime version that is no longer shown on the Portal see the language configuration guides for instructions on how to get the runtime version of your site. You can use the Azure CLI to create another site with the same runtime. Alternatively, you can use the Export **Template** button on the web app blade in the Portal to export an ARM **template** of the site. You can reuse this **template** to deploy a new site with the same runtime and configuration.

##

Linux and Windows App Service plans can now share `_____`. This limitation has been lifted from the platform and existing `_____` have been updated to support this.

%

Linux and Windows App Service plans can now share **resource groups**. This limitation has been lifted from the platform and existing **resource groups** have been updated to support this.

##

App Service limitations:

- App Service on Linux is not supported on `_____` pricing tier.
- The Azure portal shows only features that currently work for `_____` apps. As features are enabled, they're activated on the portal.
- When deployed to built-in images, your code and content are allocated a storage volume for web content, backed by Azure Storage. The disk latency of this volume is higher and more variable than the latency of the container filesystem. Apps that require heavy read-only access to content files may benefit from the `_____` option, which places files in the container filesystem instead of on the content volume.

%

- App Service on Linux is not supported on **Shared** pricing tier.
- The Azure portal shows only features that currently work for **Linux** apps. As features are enabled, they're activated on the portal.
- When deployed to built-in images, your code and content are allocated a storage volume for web content, backed by Azure Storage. The disk latency of this volume is higher and more variable than the latency of the container filesystem. Apps that require heavy read-only access to content files may benefit from the **custom container** option, which places files in the container filesystem instead of on the content volume.
