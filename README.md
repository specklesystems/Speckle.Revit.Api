# Speckle.Revit.Api
Utility repo to create the Speckle.Revit.Api package

# Prerequists
You must have Revit installed for the year that you are trying to make nugets for.

# How to use
- In your terminal of choice, navigate to the cloned repo root
- Run the command `dotnet pack /p:PackageVersion=2024 /p:DotnetVersion=net4.8 --output .` replacing the revit year and .net version with your desired version
- The .nupkg will now be created in the root folder. This can be uploaded to nuget via
  - The nuget.org UI
  - `dotnet nuget push "*.nupkg" --api-key {{your_api_key}} --source https://api.nuget.org/v3/index.json`
