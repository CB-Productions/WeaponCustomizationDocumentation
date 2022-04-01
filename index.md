## Introduction

This is the documentation for the [Weapon Loadout and Customization](https://www.unrealengine.com/marketplace/en-US/profile/CB+Productions?count=20&sortBy=effectiveDate&sortDir=DESC&start=0) available on the UE4 Marketplace.

### Changelog and future Updates

- [ ] Coming soon: More weapon assets
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

In this example we will integrate the system into the default UE4 First Person Template. This is already done in the project itself, so feel free to check out the implementation yourself.

Depending on the project you want to integrate this with, the steps will slightly differ. If your project has a dedicated weapon Blueprint we advise to implement the component in there. The UE4 First Person Template doesn't have a dedicated weapon Blueprint, but rather puts the weapon mesh directly onto the player character. So first open the `FirstPersonCharacter` Blueprint. Add the `BP_WeaponComponent` and make it a child of the existing `FP_Gun` component:

![Image](img/component.png)

Select the `FP_Gun` component and within the Details panel set *Visible* to false, so that the original weapon does not show in-game. You can adjust the position of the `Mesh1P` component to better fit the weapon. Press Play and the last selected weapon, including all the attachments will now show up:

![Image](img/fp_example.png)

The project comes already implemented. Additonaly, it allows easily customizing the weapon by returning to the main menu by pressing the M key:

![Image](img/showcase.gif)