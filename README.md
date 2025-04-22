# Woohoo.Platform.MacOS

![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/huguesv/PlatformMacOS/build-and-test.yml)
![NuGet Version](https://img.shields.io/nuget/v/Woohoo.Platform.MacOS)

Library of MacOS-only platform APIs for .NET

## Power Management

Use `PowerManagementAssertion` to manage power settings.

```csharp
using Woohoo.Platform.MacOS.PowerManagement;

// Create an instance to prevent the system from sleeping
var assertion = PowerManagementAssertion.Create("Playing Music", PowerManagementAssertionType.PreventSystemSleep);

// Dispose the instance to restore sleep settings
assertion.Dispose();
```
