---
layout: post
title:  Family Units
date:   2017-06-14 12:10:13 +1000
categories: jekyll update
assetfolder: familyunits
#from
# ![png](output_17_0.png)
#to
#![png]({{site.baseurl}}/assets/{{page.assetfolder}}/output_17_0.png)

---

### [Link to the code][familyUnitsCode]

### List of possible units in Revit

***Metric:***
   * Millimeters 
   * Cubic meters
   * Square meters 
   * Square millimeters 
   * Liters
   * Meters 
   * Meters and centimeters

***Imperial:***
   * Cubic feet
   * Square feet
   * Decimal inches
   * Feet and fractional inches
   * Square inches

***Other:***
   * General

### Project Unit types in Revit

   * Length
   * Area
   * Volume 
   * Angle 
   * Slope
   * Currency 
   * Mass Density

Our report of the mastercontent will only refer and look at length, area, volume and angle. Slope, currency and mass density is not getting looked into at the moment.

![png]({{site.baseurl}}/assets/{{page.assetfolder}}/projectUnits.png)

### Number of families using a particular unit of measurement

This shows the number of families that are using a particular unit of measurement across our master content. The unit 

![png]({{site.baseurl}}/assets/{{page.assetfolder}}/allUnits.png)

### Families that are using Metric AND imperial Units

Upon closer inspection, there were many families using both metric and imperial units of measurement. In total, there are 141 dirty families. 

***Sample of some bad families***:

<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Angle_unit_type</th>
      <th>Area_unit_type</th>
      <th>FamilyName</th>
      <th>Length_unit_type</th>
      <th>Number_unit_type</th>
      <th>Volume_unit_type</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>363</th>
      <td>Metric</td>
      <td>Evil</td>
      <td>Paper Shredder_SEQ</td>
      <td>Metric</td>
      <td>General</td>
      <td>Evil</td>
    </tr>
    <tr>
      <th>371</th>
      <td>Metric</td>
      <td>Evil</td>
      <td>Pool Cue_SEQ</td>
      <td>Metric</td>
      <td>General</td>
      <td>Evil</td>
    </tr>
    <tr>
      <th>492</th>
      <td>Metric</td>
      <td>Evil</td>
      <td>Tennis Court (indoor)_SEQ</td>
      <td>Evil</td>
      <td>General</td>
      <td>Evil</td>
    </tr>
    <tr>
      <th>499</th>
      <td>Metric</td>
      <td>Metric</td>
      <td>RearFolding_Basketball_Backstop_1937_SEQ</td>
      <td>Metric</td>
      <td>General</td>
      <td>Evil</td>
    </tr>
    <tr>
      <th>531</th>
      <td>Metric</td>
      <td>Evil</td>
      <td>Exercise Equipment - Step Machine</td>
      <td>Metric</td>
      <td>General</td>
      <td>Evil</td>
    </tr>
  </tbody>
</table>
</div>

<br />

### Number of families using an imperial or metric units

Out of the 141 dirty families that were identified above, we determined how many families were wrong from the revit's angle, area, length and volumne project units. Fortunately 100% of angles are Metric.

![png]({{site.baseurl}}/assets/{{page.assetfolder}}/categoryUnits.png)

[familyUnitsCode]: https://github.com/annisarivera/mastercontent/blob/master/working/Master%20Content%20-%20FamilyUnits.ipynb
