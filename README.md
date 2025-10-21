# Translucent Start Menu (Windows 11 Taskbar Styler)

This configuration file customizes the **Windows 11 Start Menu** using [Windhawk’s Windows 11 Start Menu Styler](https://windhawk.net/mods/windows-11-start-menu-styler).  
It refines the layout, improves transparency effects, and simplifies the UI to create a **clean and translucent Start Menu** aesthetic.

## Features

- **Translucent acrylic background** for the Start Menu  
- **Simplified layout:** hides unnecessary UI elements such as quick suggestions, extra containers, and headers  
- **Re-centered content** for a more balanced design  
- **Rounded corners** and softened folder borders  
- **Custom margins** for better visual symmetry  
- **Compact “Power” and “User” tiles** with subtle acrylic backgrounds  
- **Modernized app list appearance** with rounded corners and soft shadows  

## Preview
Preview 1:
/images/Preview_1.png

Preview 2:
/images/Preview_2.png

Preview 3:
/images/Preview_3.png

## Installation

1. **Install [Windhawk](https://windhawk.net/)**  
   Windhawk allows you to apply community mods safely to Windows 10/11.

2. **Install the [Windows 11 Start Menu Styler](https://windhawk.net/mods/windows-11-start-menu-styler)** mod inside Windhawk.

> [!TIP]
> If you want to have translucent background: Open the **Settings** menu. Under the **Theme** settings, choose **"TranslucentStartMenu"**. Click **Save settings**

3. Open the **Advanced** menu.

4. Replace **Mod Settings** with the following JSON:

<details>
  <summary>Click here to reveal the JSON</summary>
  
  ```json
   {
     "controlStyles[0].target": "Windows.UI.Xaml.Controls.Grid#UndockedRoot",
     "controlStyles[0].styles[0]": "Visibility=Visible",
     "controlStyles[0].styles[1]": "Width=348",
     "controlStyles[0].styles[2]": "Margin=132,-42,-132,0",
     "controlStyles[1].target": "Windows.UI.Xaml.Controls.Grid#AllAppsRoot",
     "controlStyles[1].styles[0]": "Visibility=Visible",
     "controlStyles[1].styles[1]": "Width=320",
     "controlStyles[1].styles[2]": "Margin=-830,-42,830,0",
     "controlStyles[2].target": "Windows.UI.Xaml.Controls.Grid#ShowMoreSuggestions",
     "controlStyles[2].styles[0]": "Visibility=Collapsed",
     "controlStyles[3].target": "Windows.UI.Xaml.Controls.Grid#SuggestionsParentContainer",
     "controlStyles[3].styles[0]": "Visibility=Collapsed",
     "controlStyles[4].target": "Windows.UI.Xaml.Controls.Grid#TopLevelSuggestionsListHeader",
     "controlStyles[4].styles[0]": "Visibility=Collapsed",
     "controlStyles[5].target": "StartDocked.SearchBoxToggleButton",
     "controlStyles[5].styles[0]": "Height=0",
     "controlStyles[5].styles[1]": "Width=0",
     "controlStyles[6].target": "Windows.UI.Xaml.Controls.Grid#TopLevelRoot > Windows.UI.Xaml.Controls.Border",
     "controlStyles[6].styles[0]": "Visibility=Collapsed",
     "controlStyles[7].target": "Windows.UI.Xaml.Controls.Button#CloseAllAppsButton",
     "controlStyles[7].styles[0]": "Visibility=Collapsed",
     "controlStyles[8].target": "StartDocked.PowerOptionsView",
     "controlStyles[8].styles[0]": "Margin=-560,0,0,0",
     "controlStyles[9].target": "StartDocked.UserTileView",
     "controlStyles[9].styles[0]": "Visibility=Visible",
     "controlStyles[9].styles[1]": "Margin=20,0,0,0",
     "controlStyles[10].target": "StartMenu.PinnedList",
     "controlStyles[10].styles[0]": "Height=504",
     "controlStyles[11].target": "StartMenu.ExpandedFolderList > Grid > Border",
     "controlStyles[11].styles[0]": "Margin=-40,0,40,0",
     "controlStyles[11].styles[1]": "Width=325",
     "controlStyles[12].target": "StartMenu.ExpandedFolderList > Grid > Grid",
     "controlStyles[12].styles[0]": "CornerRadius=8",
     "controlStyles[12].styles[1]": "Margin=-85,0,0,0",
     "controlStyles[12].styles[2]": "Width=350",
     "controlStyles[13].target": "StartMenu.ExpandedFolderList > Grid > Grid > Microsoft.UI.Xaml.Controls.PipsPager#PinnedListPipsPager",
     "controlStyles[13].styles[0]": "Margin=-15,0,0,0",
     "controlStyles[14].target": "Rectangle[4]",
     "controlStyles[14].styles[0]": "Margin=0,-20,0,0",
     "controlStyles[15].target": "Grid#TopLevelSuggestionsContainer",
     "controlStyles[15].styles[0]": "Visibility=Collapsed",
     "controlStyles[16].target": "StartDocked.AppListView",
     "controlStyles[16].styles[0]": "Margin=38,0,-38,0",
     "controlStyles[16].styles[1]": "CornerRadius=20",
     "controlStyles[17].target": "StartDocked.StartSizingFrame",
     "controlStyles[17].styles[0]": "Margin=-13,13,0,0",
     "controlStyles[17].styles[1]": "Background:=<AcrylicBrush TintColor=\"{ThemeResource CardStrokeColorDefaultSolid}\" FallbackColor=\"{ThemeResource CardStrokeColorDefaultSolid}\" TintOpacity=\"0\" TintLuminosityOpacity=\"0.5\" Opacity=\"1\"/>",
     "controlStyles[18].target": "StartDocked.NavigationPaneButton#PowerButton > Windows.UI.Xaml.Controls.Grid@CommonStates > Windows.UI.Xaml.Controls.Border#BackgroundBorder",
     "controlStyles[18].styles[0]": "Background:=<AcrylicBrush TintColor=\"{ThemeResource CardStrokeColorDefaultSolid}\" FallbackColor=\"{ThemeResource CardStrokeColorDefaultSolid}\" TintOpacity=\"0\" TintLuminosityOpacity=\"0.05\" Opacity=\"1\"/>",
     "controlStyles[18].styles[1]": "BorderBrush@Normal:=<AcrylicBrush TintColor=\"{ThemeResource SurfaceStrokeColorDefault}\" FallbackColor=\"{ThemeResource SurfaceStrokeColorDefault}\" TintOpacity=\"0\" TintLuminosityOpacity=\".1\" Opacity=\"1\"/>",
     "controlStyles[18].styles[2]": "CornerRadius=30",
     "controlStyles[18].styles[3]": "BorderThickness=0",
     "controlStyles[18].styles[4]": "Margin=0",
     "controlStyles[18].styles[5]": "BorderBrush@PointerOver:=<AcrylicBrush TintColor=\"{ThemeResource SystemAccentColor}\" FallbackColor=\"{ThemeResource SystemAccentColor}\" TintOpacity=\".8\" TintLuminosityOpacity=\".5\" Opacity=\"1\"/>",
     "theme": "TranslucentStartMenu",
     "controlStyles[19].target": "Windows.UI.Xaml.Controls.Grid#RootGrid",
     "controlStyles[19].styles[0]": "Background:=<AcrylicBrush TintColor=\"#000000\" FallbackColor=\"#000000\" TintOpacity=\"1.0\" TintLuminosityOpacity=\"0.0\" Opacity=\"0.3\"/>",
     "controlStyles[19].styles[1]": "BorderBrush:=<AcrylicBrush TintColor=\"#000000\" FallbackColor=\"#000000\" TintOpacity=\"1.0\" TintLuminosityOpacity=\"0.0\" Opacity=\"0.3\"/>",
     "controlStyles[11].styles[2]": "Background:=<AcrylicBrush TintColor=\"{ThemeResource CardStrokeColorDefaultSolid}\" FallbackColor=\"{ThemeResource CardStrokeColorDefaultSolid}\" TintOpacity=\"0\" TintLuminosityOpacity=\"0.5\" Opacity=\"1\"/>",
     "controlStyles[16].styles[2]": "Background:=<AcrylicBrush TintColor=\"{ThemeResource CardStrokeColorDefaultSolid}\" FallbackColor=\"{ThemeResource CardStrokeColorDefaultSolid}\" TintOpacity=\"0\" TintLuminosityOpacity=\"0.05\" Opacity=\"1\"/>"
   }
```
  
</details>

5. Click **Save**

6. Check if **Windows 11 Start Menu Styler** is **Enabled**

## Credits

- **[Windhawk](https://windhawk.net/)** by Ramen Software  
- **[Windows 11 Start Menu Styler](https://windhawk.net/mods/windows-11-start-menu-styler)** by Ramen Software / community contributors  
- **Config adjustments and layout design** by [Me]
