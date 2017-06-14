---
layout: post
title:  Family Types
date:   2017-06-14 12:10:13 +1000
categories: jekyll update
assetfolder: familytypes
# ![png](output_17_0.png)
#to
#![png]({{site.baseurl}}/assets/{{page.assetfolder}}/output_17_0.png)

---

### [Link to the code][familyTypesCode]

### No. of families using particular unit of measurement
The image below is a histogram that shows the number of family types there are within each family. Fortunately majority of the families in our master content have an appropriate amount of family types, though there are some that have more than 500?!

![png]({{site.baseurl}}/assets/{{page.assetfolder}}/allTypes.png)

### Number of Family Types (Highest Offenders)

"Highest Offenders" refer to families that have more than 50 family types.

![png]({{site.baseurl}}/assets/{{page.assetfolder}}/worstOff.png)

	Supply Diffuser_Sidewall                             529
    HSS_Hollow Structural Section_Pro                    333
    CISC Wide Flange Shapes_Side                         294
    CISC Wide Flange Shapes_Section                      294
    CISC Wide Flange Shapes_Top                          294
    W_Wide Flange                                        274
    W_Wide Flange_Pro                                    267
    WT_Structural Tee_Pro                                267
    WT_Structural Tee                                    267
    Table_HermanMiller_DU6ACS_RectangularTable_C_Foot    192
    CISC WT Shapes_Top                                   190
    CISC WT Shapes_Section                               190
    CISC WT Shapes_Side                                  190
    Table_HermanMiller_DU6ATS_RectangularTable_T_Foot    180
    VAV Outlet Plenum_Wye                                153
    VAV Outlet Plenum_Elbow                              153
    Louvre_Extruded_200 mm Pitch                         150

### Families with 500+ family types? whaaaaat?
The high count of family types means that these families have a Revit catalogue file attached to it. 
The code below differentiates the .txt catalogue files from the .rfa files.

### .rfa vs .txt Family Types

### .txt families
This part is a sample list that refers to family types from a .txt catalogue file.

<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: left;">
      <th></th>
      <th>FamilyFilePath</th>
      <th>FamilyName</th>
      <th>FamilyTypeName</th>
      <th>fileType</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>156</th>
      <td>Windows\Double Hung</td>
      <td>Double Hung_3LT</td>
      <td>1816</td>
      <td>txt</td>
    </tr>
    <tr>
      <th>157</th>
      <td>Windows\Double Hung</td>
      <td>Double Hung_3LT</td>
      <td>1818</td>
      <td>txt</td>
    </tr>
    <tr>
      <th>158</th>
      <td>Windows\Double Hung</td>
      <td>Double Hung_3LT</td>
      <td>1822</td>
      <td>txt</td>
    </tr>
    <tr>
      <th>159</th>
      <td>Windows\Double Hung</td>
      <td>Double Hung_3LT</td>
      <td>1824</td>
      <td>txt</td>
    </tr>
    <tr>
      <th>160</th>
      <td>Windows\Double Hung</td>
      <td>Double Hung_3LT</td>
      <td>1828</td>
      <td>txt</td>
    </tr>
  </tbody>
</table>
</div>

<br />

### .rfa families
This part is a sample list that refers to family types within the native revit family.

<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: left;">
      <th></th>
      <th>FamilyFilePath</th>
      <th>FamilyName</th>
      <th>FamilyTypeName</th>
      <th>fileType</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Windows\Special</td>
      <td>Window Round_basic</td>
      <td></td>
      <td>rfa</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Windows\Special</td>
      <td>Window Lancet_basic</td>
      <td></td>
      <td>rfa</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Windows\Special</td>
      <td>Window Arched Top_basic</td>
      <td></td>
      <td>rfa</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Windows\Special</td>
      <td>Skylight_Velux_FCM_WIN</td>
      <td></td>
      <td>rfa</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Windows\Special</td>
      <td>Skylight_Operable_WIN</td>
      <td>600 x 600mm</td>
      <td>rfa</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Windows\Special</td>
      <td>Skylight_Operable_WIN</td>
      <td>900 x 600mm</td>
      <td>rfa</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Windows\Special</td>
      <td>Skylight_Operable_WIN</td>
      <td>900 x 900mm</td>
      <td>rfa</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Windows\Special</td>
      <td>Round with Trim_WIN</td>
      <td>0610 mm Diameter</td>
      <td>rfa</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Windows\Special</td>
      <td>Round with Trim_WIN</td>
      <td>0915mm Diameter</td>
      <td>rfa</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Windows\Special</td>
      <td>Round with Trim_WIN</td>
      <td>1220mm Diameter</td>
      <td>rfa</td>
    </tr>
  </tbody>
</table>
</div>

<br />

### Number of .txt vs .rfa family types

![png]({{site.baseurl}}/assets/{{page.assetfolder}}/txtVsRfa.png)

### No. of Family Types for families with .txt files

![png]({{site.baseurl}}/assets/{{page.assetfolder}}/txtFamilies.png)

### No. of Family Types for native .rfa families

<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: left;">
      <th>FamilyName</th>
      <th>Count</th>
    </tr>
  </thead>
  <tbody style="text-align: left;">
    <tr>
      <th>1 Bay Window</th>
      <td>2</td>
    </tr>
    <tr>
      <th>1 Bay Window - Non Hosted</th>
      <td>1</td>
    </tr>
    <tr>
      <th>10P_Perimeter_Bench_FYS</th>
      <td>1</td>
    </tr>
    <tr>
      <th>115_BVNDH_WC Cubicle</th>
      <td>3</td>
    </tr>
    <tr>
      <th>12P_Meeting_FYS</th>
      <td>1</td>
    </tr>
  </tbody>
</table>
</div>

<br />

![png]({{site.baseurl}}/assets/{{page.assetfolder}}/rfaFamilies.png)

### No. of Family Types for native .rfa families (Worst Offenders)
'Worst offenders' refer to families that have more than 50 types.

<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: left;">
      <th>FamilyName</th>
      <th>Count</th>
    </tr>
  </thead>
  <tbody style="text-align: left;">
    <tr>
      <th>Timber Stud_Section_DCO</th>
      <td>80</td>
    </tr>
    <tr>
      <th>Weights equipment_SEQ</th>
      <td>67</td>
    </tr>
  </tbody>
</table>
</div>

<br />

### No. of Family Types from .txt files
This is a histogram that represents the number of family types there are in each family from .txt files.

![png]({{site.baseurl}}/assets/{{page.assetfolder}}/txtFamilies.png)

### Sample of Family Types from .txt files > 200

<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: left;">
      <th>FamilyName</th>
      <th>FamilyTypeName</th>
    </tr>
  </thead>
  <tbody style="text-align: left;">
    <tr>
      <th>CISC Wide Flange Shapes_Section</th>
      <td>294</td>
    </tr>
    <tr>
      <th>CISC Wide Flange Shapes_Side</th>
      <td>294</td>
    </tr>
    <tr>
      <th>CISC Wide Flange Shapes_Top</th>
      <td>294</td>
    </tr>
    <tr>
      <th>HSS_Hollow Structural Section_Pro</th>
      <td>333</td>
    </tr>
    <tr>
      <th>Supply Diffuser_Sidewall</th>
      <td>529</td>
    </tr>
    <tr>
      <th>WT_Structural Tee</th>
      <td>267</td>
    </tr>
    <tr>
      <th>WT_Structural Tee_Pro</th>
      <td>267</td>
    </tr>
    <tr>
      <th>W_Wide Flange</th>
      <td>274</td>
    </tr>
    <tr>
      <th>W_Wide Flange_Pro</th>
      <td>267</td>
    </tr>
  </tbody>
</table>
</div>

[familyTypesCode]: https://github.com/annisarivera/mastercontent/blob/master/working/Master%20Content%20-%20FamilyTypes.ipynb
