# Crime Simulator - Game Assemblies

This package contains **publicized and stripped** game assemblies for **Crime Simulator** mod development using **BepInEx**.

## ⚠️ Important Notes

- These assemblies are **stripped and publicized** for modding purposes only
- They are **NOT** the original game files
- Use only for BepInEx mod development with Crime Simulator
- **Requires owning the original game**

## 📦 Installation

### For Mod Projects

Add to your `.csproj` file:

```xml
<PackageReference Include="MrPurple6411.CrimeSimulator.GameAssemblies" Version="1.0.0" PrivateAssets="all" />
```

### Via .NET CLI

```bash
dotnet add package MrPurple6411.CrimeSimulator.GameAssemblies
```

## 🛠️ Usage

This package automatically provides references to:

- `Assembly-CSharp.dll` - Main game logic
- `Assembly-CSharp-firstpass.dll` - Unity first-pass scripts
- `Unity.Timeline.dll` - Unity Timeline system
- `Unity.TextMeshPro.dll` - TextMeshPro support
- `Unity.Postprocessing.Runtime.dll` - Post-processing effects
- `Steamworks.NET.dll` - Steam integration

### Accessing Private Members

All internal types are **publicized** for Harmony patching and modding access. To access previously private fields, methods, or types directly, you'll need to enable unsafe code in your project:

```xml
<PropertyGroup>
  <AllowUnsafeBlocks>true</AllowUnsafeBlocks>
</PropertyGroup>
```

**Note**: This is only required if you're directly accessing private members. Harmony patching typically doesn't require unsafe code.

## 📄 Legal

These assemblies are processed derivatives for modding purposes. You must own the original Crime Simulator game to use this package.

## 🔗 Links

- [Source Repository](https://github.com/MrPurple6411/CrimeSimulator)
- [Crime Simulator on Steam](https://store.steampowered.com)
- [BepInEx Framework](https://github.com/BepInEx/BepInEx)