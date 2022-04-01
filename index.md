## Introduction

This is the documentation for the [Weapon Loadout and Customization](https://www.unrealengine.com/marketplace/en-US/profile/CB+Productions?count=20&sortBy=effectiveDate&sortDir=DESC&start=0) available on the UE4 Marketplace.

### Changelog and future Updates

- [] Coming soon: More weapon assets
- [x] 1.0 Release

## Getting Started

### Folder structure

The asset comes with two folders. The folder `WeaponCustomization` contains the core funcationality. The folder `FirstPersonExample` contains the default UE4 First Person Template to showcase how to integrate the System into your own project. If you don't require this example, you can simply delete this folder.

Inside the `WeaponCustomization` folder there are several important sub-folders:

| Folder | Description |
| --- | --- |
| Blueprints | Files for the core functionality |
| DataAssets | Contains all the DataAssets for Weapons and Weapon Attachments |
| UI | Contains all the UMG widgets that are used |
| WeaponAssets | Contains all the assets (meshes, textures, materials) | 

## Integration into another Project

The integration into another project is kept simple. For a basic integration only one component needs to be added to the existing weapon or character class.

In this example we will integrate 

![Image](img/component.PNG)

