[! [license] [license-badge]] [LICENSE]

### Presentation

Displays on the OpenCart control panel the sales map in Brazil with the orders divided by the Brazilian states.

#### Important:

If you are using a version of OpenCart below 2.3, you will be installing a modification.

If you are using version 2.3 or 3.0, you are installing an extension.

### Installation

 1. Access the link: https://www.opencart.com/index.php?route=marketplace/extension/info&extension_id=22375.
 2. Find the most current version and compatible with your version of OpenCart and download it.
 3. In the store administration, access the menu "** Extensions → Installer **" (Extensions → Installer).
 4. On the installer page, click the "** Upload **" button and select the file '** mapa-vendas-brasil.ocmod.zip **' (which you downloaded from this repository), and wait for the installation to complete automatic.
 5. After installation, if you are using an OpenCart version lower than 2.3, access the menu "** Extensions → Modifications **" (Extensions → Modifications) and click the "** Update **" button (Refresh) to that the modification installed and increased in the store, remembering that it is not the Update button on your browser, but the Update button in blue color next to the orange and red button on the OpenCart screen.
 6. If you are using version 2.3 or 3.0 of OpenCart, access the menu "** Extensions → Extensions **", filter for "** Panels **", find the extension "** Sales map in Brazil **" , click the "** Install **" button, then the "** Edit **" button, in the "** Width / Columns **" field, select ** 6 **, in the "** Situation **" field select ** Enabled **, in the "** Position **" field, fill in ** 5 **, and click the "** Save **" button, then locate the extension "** Geographic sales map **" , click the "** Edit **" button, in the "** Situation **" field select ** Disabled **, and click the "** Save **" button.

### Uninstallation

If you are using an OpenCart version lower than 2.3, in the store administration, access the menu ** Extensions → Modifications ** (Extensions → Modifications), select the modification with the name '** Sales map in Brazil **', then click the "** Delete **" button (Delete), and the "** Update **" button (Refresh).

If you are using version 2.3 or 3.0, access the menu "** Extensions → Extensions **", filter for "** Panels **", find the extension "** Sales map in Brazil **", click the button "** Delete **" (Delete), then find the extension "** Geographic sales map **", click on the "** Edit **" button, in the "** Situation **" field select ** Enabled **, and click the "** Save **" button.

### Update

Access the store administration and perform the Uninstall procedure, then perform the Installation procedure, according to your version of OpenCart.

### Correction for OpenCart 2.3.0.0, 2.3.0.1 and 2.3.0.2:

In these versions of OpenCart, there is a bug that prevents you from opening the settings of new extensions of type "Panel" after clicking the Install button, to fix the bug, do the following:

- Edit the file below (preferably with the Notepad ++ editor):

admin / controller / extension / extension / ** dashboard.php **

- Locate the line below:

`` $ this-> model_extension_extension-> install ('dashboard', 'dashboard_'. $ this-> request-> get ['extension']); ``

- And replace with:

`` $ this-> model_extension_extension-> install ('dashboard', $ this-> request-> get ['extension']); ``

- Locate the line below:

`` $ this-> model_extension_extension-> uninstall ('dashboard', 'dashboard_'. $ this-> request-> get ['extension']); ``

- And replace with:

`` $ this-> model_extension_extension-> uninstall ('dashboard', $ this-> request-> get ['extension']); ``

Now save the changes to the file, and install the extension again that the problem will be solved.

### Doubts

OCMOD (OpenCart Modification) is native to OpenCart, that is, it is not necessary to install any add-on in OpenCart to use modifications or extensions in the OCMOD format, for more information about OCMOD, follow the link for more information:

https://github.com/opencart/opencart/wiki/Modification-System

[license-badge]: https://img.shields.io/badge/licença-GPLv3-blue.svg
[LICENSE]: ./LICENSE 
