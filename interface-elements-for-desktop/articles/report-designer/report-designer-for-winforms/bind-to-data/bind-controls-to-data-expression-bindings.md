---
title: Bind Report Controls to Data (Expression Bindings)
author: Anna Gubareva
---
# Bind Report Controls to Data (Expression Bindings)

> [!Warning]
> Use the approach below if expression bindings **are enabled** in the Report Designer (the [Property Grid](../report-designer-tools/ui-panels/property-grid.md) provides the **Expressions** ![](../../../../images/eurd-win-property-grid-expressions-icon.png) tab ).
>
> See [Bind Report Controls to Data (Data Bindings)](bind-controls-to-data-data-bindings.md) if expression bindings **are not enabled** in the Report Designer (the [Property Grid](../report-designer-tools/ui-panels/property-grid.md) does not provide the **Expressions** ![](../../../../images/eurd-win-property-grid-expressions-icon.png) tab).

You can use the following approaches to include a data source's information in your report:

* [Use the Field List](#use-the-field-list)
* [Use the Smart Tag](#use-the-smart-tag)
* [Use the Property Grid](#use-the-property-grid)

## Use the Field List

After you [bind your report to data](../bind-to-data.md), the [Field List](../report-designer-tools/ui-panels/field-list.md) panel displays the data source's hierarchy and provides access to the available data fields. 

Drop a data field from this panel onto a report's surface to create a new report control bound to the corresponding field.

![eurd-win-field-list-drop-fields](../../../../images/eurd-win-field-list-drop-fields.png)

Drop a data field onto an existing control to bind this control to the corresponding field.

![eurd-win-field-list-drop-field-to-control](../../../../images/eurd-win-field-list-drop-field-to-control.png)

You can do one of the following to create a data-bound control of a specific type:

* Hold down the SHIFT key and drop a data field onto a report's surface.
* Right-click a corresponding data field and drop it onto a report's surface.

This invokes a context menu that enables you to select which control to create.

![eurd-win-fieldlist-create-specific-contols](../../../../images/eurd-win-fieldlist-create-specific-contols.png)

You can also drop an entire data table onto a report to create a [Table](../use-report-elements/use-tables.md) control with its cells bound to the corresponding data table fields. 

![eurd-win-field-list-drop-table](../../../../images/eurd-win-field-list-drop-table.png)

To select multiple fields in the Field List, hold CTRL or SHIFT and click the fields. Drop these fields onto a report to create a new table.

![design-time-field-list-drop-multiple-fields](../../../../images/eurd-win-list-drop-multiple-fields.png)

## Use the Smart Tag

Click a control's smart tag, expand the **Expression** drop-down list and select a data field.

![](../../../../images/eurd-win-label-bind-to-data-field.png)

You can also click the **Expression** option's ellipsis button to invoke the **Expression Editor**. This editor allows you to construct a complex binding expression with two or more data fields and various functions. See [Expression Syntax](../use-expressions/expression-syntax.md) for more information.
 
![](../../../../images/eurd-win-label-expression-binding.png)


## Use the Property Grid

Select a report control and switch to the **Expressions** tab in the [Property Grid](../report-designer-tools/ui-panels/property-grid.md). Click the **Text** property's ellipsis button and construct a binding  [expression](../use-expressions/expression-syntax.md) in the invoked **Expression Editor**.

![](../../../../images/eurd-win-property-grid-expressions.png)

You can use the same approach to specify expressions for all the control properties. See [Shape Report Data](../shape-report-data/shape-data-expression-bindings.md) for more tutorials.

