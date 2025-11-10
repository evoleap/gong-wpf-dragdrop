# .NET 8.0 Upgrade Plan

## Execution Steps

Execute steps below sequentially one by one in the order they are listed.

1. Validate that a .NET 8.0 SDK required for this upgrade is installed on the machine and if not, help to get it installed.
2. Ensure that the SDK version specified in global.json files is compatible with the .NET 8.0 upgrade.
3. Upgrade GongSolutions.Wpf.DragDrop\GongSolutions.Wpf.DragDrop.csproj
4. Upgrade Examples\NorthwindExample\NorthwindExample.csproj
5. Upgrade Examples\DefaultsExample\DefaultsExample.csproj
6. Upgrade GongSolutions.Wpf.DragDrop.UnitTests\GongSolutions.Wpf.DragDrop.UnitTests.csproj
7. Run unit tests to validate upgrade in the project: GongSolutions.Wpf.DragDrop.UnitTests\GongSolutions.Wpf.DragDrop.UnitTests.csproj

## Settings

This section contains settings and data used by execution steps.

### Project upgrade details

This section contains details about each project upgrade and modifications that need to be done in the project.

#### GongSolutions.Wpf.DragDrop\GongSolutions.Wpf.DragDrop.csproj modifications

Project properties changes:
  - Convert project to SDK-style format
  - Target framework should be changed from `net472` to `net8.0-windows`

#### Examples\NorthwindExample\NorthwindExample (NET4).csproj modifications

Project properties changes:
  - Convert project to SDK-style format
  - Target framework should be changed from `net48` to `net8.0-windows`

#### Examples\DefaultsExample\DefaultsExample.csproj modifications

Project properties changes:
  - Convert project to SDK-style format
  - Target framework should be changed from `net48` to `net8.0-windows`

#### GongSolutions.Wpf.DragDrop.UnitTests\GongSolutions.Wpf.DragDrop.UnitTests.csproj modifications

Project properties changes:
  - Convert project to SDK-style format
  - Target framework should be changed from `net48` to `net8.0`
