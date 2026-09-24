# How to Customize the Axis Label Format Based on Culture in Blazor Charts

## Overview

This sample demonstrates how to format chart axis labels according to the application's active culture settings in Syncfusion [Blazor Charts](https://www.syncfusion.com/blazor-components/blazor-charts). The implementation uses application localization together with chart axis formatting so that numeric values are displayed using culture-specific currency symbols and formatting rules.

In the sample, the application is configured to use the `en-IE` culture and the chart's primary Y-axis is formatted as currency. This approach ensures that chart data is presented consistently with the regional settings expected by users.

## Key Features

- Uses the `SfChart` component to render chart data.
- Configures a spline series through `ChartSeries` with `Type="ChartSeriesType.Spline"`.
- Binds chart data using the `DataSource`, `XName`, and `YName` properties.
- Formats axis labels using the `ChartPrimaryYAxis` `LabelFormat` property.
- Demonstrates currency formatting through `LabelFormat="c"`.
- Shows culture-aware rendering by configuring request localization with:
  - `app.UseRequestLocalization("en-IE")`
- Uses a strongly typed `ChartData` model containing:
  - `double X`
  - `double Y`

## Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)
- [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download this repository.
2. Open the project file located inside the `Culture` folder.
3. Restore all NuGet packages.
4. Build the project.
5. Run the application using `Ctrl+F5`.

**Visual Studio Code**

1. Clone or download this repository.
2. Open the repository folder in Visual Studio Code.
3. Open the integrated terminal.
4. Navigate to the project directory.

```bash
cd Culture
dotnet restore
dotnet run
```

5. Open the local URL displayed in the terminal after the application starts.

## Project Structure

- `Pages/Index.razor` - Implements the `SfChart` component, chart data model, data collection, spline series configuration, and axis label formatting.
- `Program.cs` - Configures application localization using `UseRequestLocalization("en-IE")`.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- Refer to the official Chart Axis API documentation: https://help.syncfusion.com/cr/blazor/Syncfusion.Blazor.Charts.ChartAxis.html

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.