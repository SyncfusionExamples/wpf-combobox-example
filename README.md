# WPF ComboBoxAdv Example
## Overview
This sample demonstrates how to get started with using the Syncfusion WPF ComboBoxAdv control. ComboBoxAdv is an enhanced combo box control that provides additional styling and functionality compared to the standard WPF ComboBox.

## Creating the Project
Follow these steps to create a new WPF project in Visual Studio and display the ComboBoxAdv control.

### Adding the Control Manually in XAML
**Steps:**
1. Add the required assembly reference:
   - Syncfusion.Shared.WPF
     
2. Import the Syncfusion WPF schema in your XAML page:
```XAML
xmlns:syncfusion="http://schemas.syncfusion.com/wpf"
```

3. Declare the ComboBoxAdv control:
```
<Grid>
    <syncfusion:ComboBoxAdv Height="30" Width="150" />
</Grid>
```

## Adding the Control Manually in C#
**Steps:**
1. Add the required assembly reference:
   - Syncfusion.Shared.WPF

2. Import the namespace:
```C#
using Syncfusion.Windows.Tools.Controls;
```
3. Create and configure the ComboBoxAdv control:
``` C#
public partial class MainWindow : Window
{
    public MainWindow()
    {
        InitializeComponent();
        ComboBoxAdv comboBoxAdv = new ComboBoxAdv();
        comboBoxAdv.Height = 30;
        comboBoxAdv.Width = 150;
        comboBoxAdv.DefaultText = "Choose Items";
        this.Content = comboBoxAdv;
    }
}

```
## How to Run This Application
- Clone the wpf-combobox-example repository.
- Open the solution in Visual Studio.
- Build and run the project to view the output of ComboBoxAdv.

## Troubleshooting
### Path Too Long Exception
If you encounter a "path too long" error while building the project:
- Close Visual Studio.
- Rename the repository folder to a shorter name.
- Reopen and build the project.
