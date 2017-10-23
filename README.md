# Find Active Debuggers

This package adds a method and action to locate active debuggers in Aras Method items.

## History

Release | Notes
--------|--------
[v2.0](https://github.com/ArasLabs/find-active-debuggers/releases/tag/v2.0) | Adds support for JavaScript methods.
[v1.0](https://github.com/ArasLabs/find-active-debuggers/releases/tag/v1.0) | First release. only supports server-side methods. Though built and tested using Aras 11.0 SP7, this project may function in older releases of Aras 11.0 and Aras 10.0.

#### Supported Aras Versions

Project | Aras
--------|------
[v2.0](https://github.com/ArasLabs/find-active-debuggers/releases/tag/v2.0) | 11.0 SP5, 11.0 SP7, 11.0 SP9
[v1.0](https://github.com/ArasLabs/find-active-debuggers/releases/tag/v1.0) | 11.0 SP5, 11.0 SP7

## Installation

#### Important!
**Always back up your code tree and database before applying an import package or code tree patch!**

### Pre-requisites

1. Aras Innovator installed (version 11.0 SPx preferred)
2. Aras Package Import tool
3. FindActiveDebuggers import package

### Install Steps

1. Backup your database and store the BAK file in a safe place.
2. Open up the Aras Package Import tool.
3. Enter your login credentials and click **Login**
    * _Note: You must login as root for the package import to succeed!_
4. Enter the package name in the TargetRelease field.
    * Optional: Enter a description in the Description field.
5. Enter the path to your local `..\FindActiveDebuggers\Import\imports.mf` file in the Manifest File field.
6. Select **FindActiveDebuggers** in the Available for Import field.
7. Select Type = **Merge** and Mode = **Thorough Mode**.
8. Click **Import** in the top left corner.
9. Close the Aras Package Import tool.
10. (Optional) Execute the contents of [Data\testData.xml](./Data/testData.xml) in Nash or AML Studio to add sample data to your database for testing.

You are now ready to login to Aras and try out the Find Active Debuggers action.

## Usage

1. Log in to Aras as admin.
2. Click **Actions > Find Active Debuggers** in the main menu.

The Find Active Debuggers action will display a window with the results of the report. The window will show a list of methods containing an active debugger statement and a search criteria string that you can copy into the Method main grid search toolbar.

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

For more information on contributing to this project, another Aras Labs project, or any Aras Community project, shoot us an email at araslabs@aras.com.

## Credits

Original code written by Mike Ghizzoni for Aras Corporation Support.

Documented and published by Eli Donahue for Aras Labs. @EliJDonahue

Contributors:
* @mptap

## License

Aras Labs projects are published to Github under the MIT license. See the [LICENSE file](./LICENSE.md) for license rights and limitations.
