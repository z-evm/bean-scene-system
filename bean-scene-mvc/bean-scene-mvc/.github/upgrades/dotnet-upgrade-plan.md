# .NET 9.0 Upgrade Plan

## Execution Steps

Execute steps below sequentially one by one in the order they are listed.

1. Validate that a .NET 9.0 SDK required for this upgrade is installed on the machine and if not, help to get it installed.
2. Ensure that the SDK version specified in global.json files is compatible with the .NET 9.0 upgrade.
3. Upgrade BeanScene\BeanScene.csproj

## Settings

### Aggregate NuGet packages modifications across all projects

NuGet packages used across all selected projects or their dependencies that need version update in projects that reference them.

| Package Name         | Current Version | New Version | Description           |
|:-------------------------------------------------------|:---------------:|:-----------:|:----------------------------------------------|
| Microsoft.AspNetCore.Diagnostics.EntityFrameworkCore  |   8.0.10        |  9.0.10     | Recommended for .NET 9.0    |
| Microsoft.AspNetCore.Identity.EntityFrameworkCore     |   8.0.10        |  9.0.10     | Recommended for .NET 9.0      |
| Microsoft.AspNetCore.Identity.UI             |   8.0.10        |  9.0.10     | Recommended for .NET 9.0        |
| Microsoft.EntityFrameworkCore.Sqlite         |   8.0.10      |  9.0.10     | Recommended for .NET 9.0        |
| Microsoft.EntityFrameworkCore.SqlServer   |   8.0.10  |  9.0.10     | Recommended for .NET 9.0           |
| Microsoft.EntityFrameworkCore.Tools                   |   8.0.10   |  9.0.10     | Recommended for .NET 9.0     |

### Project upgrade details

#### BeanScene\BeanScene.csproj modifications

Project properties changes:
  - Target framework should be changed from `net8.0` to `net9.0`

NuGet packages changes:
  - Microsoft.AspNetCore.Diagnostics.EntityFrameworkCore should be updated from `8.0.10` to `9.0.10` (*recommended for .NET 9.0*)
  - Microsoft.AspNetCore.Identity.EntityFrameworkCore should be updated from `8.0.10` to `9.0.10` (*recommended for .NET 9.0*)
  - Microsoft.AspNetCore.Identity.UI should be updated from `8.0.10` to `9.0.10` (*recommended for .NET 9.0*)
  - Microsoft.EntityFrameworkCore.Sqlite should be updated from `8.0.10` to `9.0.10` (*recommended for .NET 9.0*)
  - Microsoft.EntityFrameworkCore.SqlServer should be updated from `8.0.10` to `9.0.10` (*recommended for .NET 9.0*)
  - Microsoft.EntityFrameworkCore.Tools should be updated from `8.0.10` to `9.0.10` (*recommended for .NET 9.0*)