---
title:ChartBuilder
slug:aspnetmvc-kendo.mvc.ui.fluent.chartbuilder
publish:true
---

# Kendo.Mvc.UI.Fluent.ChartBuilder
Defines the fluent interface for configuring the !:Chart{T} component.



## Methods

### Events(`System.Action<Kendo.Mvc.UI.Fluent.ChartEventBuilder>`)
Configures the client-side events.


#### Parameters

##### configurator System.Action<[Kendo.Mvc.UI.Fluent.ChartEventBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartEventBuilder)>
The client events configuration action.




#### Example (ASPX)
    <%= Html.Kendo().Chart()
    .Name("Chart")
    .Events(events => events
        .OnLoad("onLoad")
    )
    %>


### RenderAs(`Kendo.Mvc.UI.RenderingMode`)
Sets the preferred rendering engine.
            If it is not supported by the browser, the Chart will switch to the first available mode.


#### Parameters

##### renderAs [Kendo.Mvc.UI.RenderingMode](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI/RenderingMode)
The preferred rendering engine.





### Theme(`System.String`)
Sets the theme of the chart.


#### Parameters

##### theme `System.String`
The Chart theme.




#### Example (ASPX)
    <%= Html.Kendo().Chart()
    .Name("Chart")
    .Theme("Telerik")
    %>


### ChartArea(`System.Action<Kendo.Mvc.UI.Fluent.ChartAreaBuilder>`)
Sets the Chart area.


#### Parameters

##### configurator System.Action<[Kendo.Mvc.UI.Fluent.ChartAreaBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartAreaBuilder)>
The Chart area.




#### Example (ASPX)
    <%= Html.Kendo().Chart()
    .Name("Chart")
    .ChartArea(chartArea => chartArea.margin(20))
    %>


### PlotArea(`System.Action<Kendo.Mvc.UI.Fluent.PlotAreaBuilder>`)
Sets the Plot area.


#### Parameters

##### configurator System.Action<[Kendo.Mvc.UI.Fluent.PlotAreaBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/PlotAreaBuilder)>
The Plot area.




#### Example (ASPX)
    <%= Html.Kendo().Chart()
    .Name("Chart")
    .PlotArea(plotArea => plotArea.margin(20))
    %>


### Title(`System.String`)
Sets the title of the chart.


#### Parameters

##### title `System.String`
The Chart title.




#### Example (ASPX)
    <%= Html.Kendo().Chart()
    .Name("Chart")
    .Title("Yearly sales")
    %>


### Title(`System.Action<Kendo.Mvc.UI.Fluent.ChartTitleBuilder>`)
Defines the title of the chart.


#### Parameters

##### configurator System.Action<[Kendo.Mvc.UI.Fluent.ChartTitleBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartTitleBuilder)>
The configuration action.




#### Example (ASPX)
    <%= Html.Kendo().Chart()
    .Name("Chart")
    .Title(title => title.Text("Yearly sales"))
    %>


### Legend(`System.Boolean`)
Sets the legend visibility.


#### Parameters

##### visible `System.Boolean`
A value indicating whether to show the legend.




#### Example (ASPX)
    <%= Html.Kendo().Chart()
    .Name("Chart")
    .Legend(false)
    %>


### Legend(`System.Action<Kendo.Mvc.UI.Fluent.ChartLegendBuilder>`)
Configures the legend.


#### Parameters

##### configurator System.Action<[Kendo.Mvc.UI.Fluent.ChartLegendBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartLegendBuilder)>
The configuration action.




#### Example (ASPX)
    <%= Html.Kendo().Chart()
    .Name("Chart")
    .Legend(legend => legend.Visible(true).Position(ChartLegendPosition.Bottom))
    %>


### Series(`System.Action<Kendo.Mvc.UI.Fluent.ChartSeriesFactory<T>>`)
Defines the chart series.


#### Parameters

##### configurator System.Action<[Kendo.Mvc.UI.Fluent.ChartSeriesFactory](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartSeriesFactory)<T>>
The add action.




#### Example (ASPX)
    <%= Html.Kendo().Chart(Model)
    .Name("Chart")
    .Series(series =>
    {
        series.Bar(s => s.SalesAmount);
    })
    %>


### SeriesDefaults(`System.Action<Kendo.Mvc.UI.Fluent.ChartSeriesDefaultsBuilder<T>>`)
Defines the options for all chart series of the specified type.


#### Parameters

##### configurator System.Action<[Kendo.Mvc.UI.Fluent.ChartSeriesDefaultsBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartSeriesDefaultsBuilder)<T>>
The configurator.




#### Example (ASPX)
    <%= Html.Kendo().Chart(Model)
    .Name("Chart")
    .SeriesDefaults(series => series.Bar().Stack(true))
    %>


### Panes(`System.Action<Kendo.Mvc.UI.Fluent.ChartPanesFactory>`)
Defines the chart panes.


#### Parameters

##### configurator System.Action<[Kendo.Mvc.UI.Fluent.ChartPanesFactory](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartPanesFactory)>
The add action.




#### Example (ASPX)
    <%= Html.Kendo().Chart(Model)
    .Name("Chart")
    .Panes(panes =>
    {
        panes.Add("volume");
    })
    %>


### AxisDefaults(`System.Action<Kendo.Mvc.UI.Fluent.ChartAxisDefaultsBuilder<T>>`)
Defines the options for all chart axes of the specified type.


#### Parameters

##### configurator System.Action<[Kendo.Mvc.UI.Fluent.ChartAxisDefaultsBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartAxisDefaultsBuilder)<T>>
The configurator.




#### Example (ASPX)
    <%= Html.Kendo().Chart(Model)
    .Name("Chart")
    .AxisDefaults(axisDefaults => axisDefaults.MinorTickSize(5))
    %>


### CategoryAxis(`System.Action<Kendo.Mvc.UI.Fluent.ChartCategoryAxisBuilder<T>>`)
Configures the category axis


#### Parameters

##### configurator System.Action<[Kendo.Mvc.UI.Fluent.ChartCategoryAxisBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartCategoryAxisBuilder)<T>>
The configurator




#### Example (ASPX)
    <%= Html.Kendo().Chart(Model)
    .Name("Chart")
    .CategoryAxis(axis => axis
        .Categories(s => s.DateString)
    )
    %>


### ValueAxis(`System.Action<Kendo.Mvc.UI.Fluent.ChartValueAxisFactory<T>>`)
Defines value axis options


#### Parameters

##### configurator System.Action<[Kendo.Mvc.UI.Fluent.ChartValueAxisFactory](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartValueAxisFactory)<T>>
The configurator




#### Example (ASPX)
    <%= Html.Kendo().Chart(Model)
    .Name("Chart")
    .ValueAxis(a => a.Numeric().TickSize(4))
    %>


### XAxis(`System.Action<Kendo.Mvc.UI.Fluent.ChartValueAxisFactory<T>>`)
Defines X-axis options for scatter charts


#### Parameters

##### configurator System.Action<[Kendo.Mvc.UI.Fluent.ChartValueAxisFactory](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartValueAxisFactory)<T>>
The configurator




#### Example (ASPX)
    <%= Html.Kendo().Chart(Model)
    .Name("Chart")
    .XAxis(a => a.Numeric().Max(4))
    %>


### YAxis(`System.Action<Kendo.Mvc.UI.Fluent.ChartValueAxisFactory<T>>`)
Configures Y-axis options for scatter charts.


#### Parameters

##### configurator System.Action<[Kendo.Mvc.UI.Fluent.ChartValueAxisFactory](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartValueAxisFactory)<T>>
The configurator




#### Example (ASPX)
    <%= Html.Kendo().Chart(Model)
    .Name("Chart")
    .YAxis(a => a.Numeric().Max(4))
    %>


### DataSource(`System.Action<Kendo.Mvc.UI.Fluent.ReadOnlyAjaxDataSourceBuilder<T>>`)
Data Source configuration


#### Parameters

##### configurator System.Action<[Kendo.Mvc.UI.Fluent.ReadOnlyAjaxDataSourceBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ReadOnlyAjaxDataSourceBuilder)<T>>
Use the configurator to set different data binding options.




#### Example (ASPX)
    <%= Html.Kendo().Chart()
    .Name("Chart")
    .DataSource(ds =>
    {
        ds.Ajax().Read(r => r.Action("SalesData", "Chart"));
    })
    %>


### AutoBind(`System.Boolean`)
Enables or disables automatic binding.


#### Parameters

##### autoBind `System.Boolean`
Gets or sets a value indicating if the chart
            should be data bound during initialization.
            The default value is true.




#### Example (ASPX)
    <%= Html.Kendo().Chart()
    .Name("Chart")
    .DataSource(ds =>
    {
        ds.Ajax().Read(r => r.Action("SalesData", "Chart"));
    })
    .AutoBind(false)
    %>


### SeriesColors(`System.Collections.Generic.IEnumerable<System.String>`)
Sets the series colors.


#### Parameters

##### colors `System.Collections.Generic.IEnumerable<System.String>`
A list of the series colors.




#### Example (ASPX)
    <%= Html.Kendo().Chart()
    .Name("Chart")
    .SeriesColors(new string[] { "#f00", "#0f0", "#00f" })
    %>


### SeriesColors(`System.String[]`)
Sets the series colors.


#### Parameters

##### colors `System.String[]`
The series colors.




#### Example (ASPX)
    <%= Html.Kendo().Chart()
    .Name("Chart")
    .SeriesColors("#f00", "#0f0", "#00f")
    %>


### Tooltip(`System.Action<Kendo.Mvc.UI.Fluent.ChartTooltipBuilder>`)
Use it to configure the data point tooltip.


#### Parameters

##### configurator System.Action<[Kendo.Mvc.UI.Fluent.ChartTooltipBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartTooltipBuilder)>
Use the configurator to set data tooltip options.




#### Example (ASPX)
    <%= Html.Kendo().Chart()
    .Name("Chart")
    .Tooltip(tooltip =>
    {
        tooltip.Visible(true).Format("{0:C}");
    })
    %>


### Tooltip(`System.Boolean`)
Sets the data point tooltip visibility.


#### Parameters

##### visible `System.Boolean`
A value indicating if the data point tooltip should be displayed.
            The tooltip is not visible by default.




#### Example (ASPX)
    <%= Html.Kendo().Chart()
    .Name("Chart")
    .Tooltip(true)
    %>


### Transitions(`System.Boolean`)
Enables or disabled animated transitions on initial load and refresh.


#### Parameters

##### transitions `System.Boolean`
A value indicating if transition animations should be played.




#### Example (ASPX)
    <%= Html.Kendo().Chart()
    .Name("Chart")
    .Transitions(false)
    %>



