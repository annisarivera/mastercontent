---
layout: post
title:  Family Parameters
date:   2017-06-14 12:10:13 +1000
categories: jekyll update
assetfolder: familyparameters
# ![png](output_17_0.png)
#to
#![png]({{site.baseurl}}/assets/{{page.assetfolder}}/output_17_0.png)

---

### [Link to the code][familyParametersCode]

### Number of parameters within families
This is a histogram that shows the number of parameters families use across the master content. What can be seen from the image below is that there are families that have more than 200 families.

![png]({{site.baseurl}}/assets/{{page.assetfolder}}/allParameters.png)

### Number of parameters within families (High offenders)
High offenders refer to families with more than 100 parameters. This is only a sample list. 

<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: left;">
      <th>FamilyName</th>
      <th>count</th>
    </tr>
  </thead>
  <tbody style="text-align: left;">
    <tr>
      <th>Accordion_Double_DOR</th>
      <td>128</td>
    </tr>
    <tr>
      <th>Accordion_Single_DOR</th>
      <td>125</td>
    </tr>
    <tr>
      <th>Base Cabinet_Corner_LShape_CAS</th>
      <td>184</td>
    </tr>
    <tr>
      <th>Base Cabinet_Dishwasher_CAS</th>
      <td>161</td>
    </tr>
    <tr>
      <th>Base Cabinet_Door with Drawer_CAS</th>
      <td>171</td>
    </tr>
    <tr>
      <th>Base Cabinet_Double_CAS</th>
      <td>184</td>
    </tr>
    <tr>
      <th>Base Cabinet_Drawer_1_CAS</th>
      <td>166</td>
    </tr>
  </tbody>
</table>
</div>

<br />

### Are the parameters shared parameters?
The sample list below shows whether the parameters used by families are from the shared parameter list, defaults or user created.

<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: left;">
      <th></th>
      <th>FamilyFilePath</th>
      <th>FamilyName</th>
      <th>ParameterName</th>
      <th>BVNparam</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Windows\Structural</td>
      <td>Window_Square Opening_WIN</td>
      <td>Analytic Construction</td>
      <td>False</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Windows\Structural</td>
      <td>Window_Square Opening_WIN</td>
      <td>Assembly Code</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Windows\Structural</td>
      <td>Window_Square Opening_WIN</td>
      <td>Construction Type</td>
      <td>False</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Windows\Structural</td>
      <td>Window_Square Opening_WIN</td>
      <td>Cost</td>
      <td>False</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Windows\Structural</td>
      <td>Window_Square Opening_WIN</td>
      <td>Description</td>
      <td>False</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Windows\Structural</td>
      <td>Window_Square Opening_WIN</td>
      <td>Heat Transfer Coefficient (U)</td>
      <td>False</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Windows\Structural</td>
      <td>Window_Square Opening_WIN</td>
      <td>Model</td>
      <td>False</td>
    </tr>
  </tbody>
</table>
</div>

<br />

### Number of parameters that are using SP vs non-SP

![png]({{site.baseurl}}/assets/{{page.assetfolder}}/spVsNonSp.png)

### Families that are only using shared parameters

<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: left;">
      <th></th>
      <th>FamilyName</th>
      <th>ParameterName</th>
      <th>BVNparam</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>32</th>
      <td>Window_Round Opening_WIN</td>
      <td>Radius</td>
      <td>True</td>
    </tr>
    <tr>
      <th>58</th>
      <td>Window Round_basic</td>
      <td>Material Frame</td>
      <td>True</td>
    </tr>
    <tr>
      <th>87</th>
      <td>Window Lancet_basic</td>
      <td>Material Frame</td>
      <td>True</td>
    </tr>
    <tr>
      <th>115</th>
      <td>Window Arched Top_basic</td>
      <td>Material Frame</td>
      <td>True</td>
    </tr>
    <tr>
      <th>165</th>
      <td>Skylight_Operable_WIN</td>
      <td>Glazing</td>
      <td>True</td>
    </tr>
    <tr>
      <th>166</th>
      <td>Skylight_Operable_WIN</td>
      <td>Glazing Material</td>
      <td>True</td>
    </tr>
    <tr>
      <th>172</th>
      <td>Skylight_Operable_WIN</td>
      <td>Mullion Height</td>
      <td>True</td>
    </tr>
    <tr>
      <th>184</th>
      <td>Skylight_Operable_WIN</td>
      <td>Window Blind Type</td>
      <td>True</td>
    </tr>
    <tr>
      <th>185</th>
      <td>Skylight_Operable_WIN</td>
      <td>Window Jockey Sash</td>
      <td>True</td>
    </tr>
    <tr>
      <th>186</th>
      <td>Skylight_Operable_WIN</td>
      <td>Window Louvre</td>
      <td>True</td>
    </tr>
  </tbody>
</table>
</div>

<br />

### No. of SP parameters vs non-BVN SP parameters of each family

<div>
<table border="1" class="dataframe">
  <thead>
    <tr>
    </tr>
    <tr style="text-align: left;">
      <th>FamilyName</th>
      <th>BVNparam</th>
      <th>count</th>
    </tr>
  </thead>
  <tbody style="text-align: left;">
    <tr>
      <th rowspan="2" valign="top">1 Bay Window</th>
      <th>False</th>
      <td>33</td>
    </tr>
    <tr>
      <th>True</th>
      <td>1</td>
    </tr>
    <tr>
      <th>1 Bay Window - Non Hosted</th>
      <th>False</th>
      <td>30</td>
    </tr>
    <tr>
      <th>10P_Perimeter_Bench_FYS</th>
      <th>False</th>
      <td>17</td>
    </tr>
    <tr>
      <th>115_BVNDH_WC Cubicle</th>
      <th>False</th>
      <td>25</td>
    </tr>
  </tbody>
</table>
</div>

<br />

### SP's that are not used (dead parameters)

     A3 Scale
     AS1482 Tolerance
     Acoustic Rating Rw
     Adaptable
     Additional Info- Fourth Line
     Area Colour
     BVN Alphabet
     Balcony Area
     Category Color
     Ceiling Acoustic Rating
     Client Project Number
     Configured By
     Consultant 01
     Consultant 01 Details
     Consultant 02
     Consultant 02 Details
     Consultant 03
     Consultant 03 Details
     Consultant 04
     Consultant 04 Details
     Consultant 05
     Consultant 05 Details
     Copyright \xc2\xa9
     Core Name
     Discipline
     Expected Lifespan (Years)
     Ext Frame_Offset EQUAL Host Wall thickness_i
     Flux Id
     HsbType
     Ideate BIMLink
     ItemCode_2
     ItemDescription_2
     ItemGroup_2
     Level - Second Line
     Lining_"Opposite Side"
     Lining_"Placement Side"
     Maintenance Schedule (Months)
     Original Model By
     Package
     Panel 1 Height
     Panel 1 Width
     Place in Structural Wall_i
     Project Manager
     Project Managers Details
     Project Stage
     Project Stage Code
     Project Type
     Room Colour
     SEPP 65 - Cross Ventilation
     SEPP 65 - Solar Access
     SEPP 65 - South Aspect
     SEPP65 - Daylight Access
     SEPP65_Cross Ventilation
     SEPP65_Solar Access
     SEPP65_South Facing
     SR Document GUID
     SR View Calculation Settings
     STF_Parking_Disabled_YesNo_t
     STF_Parking_Wheelstop_Depth_t
     STF_Parking_Wheelstop_Height_t
     STF_Parking_Wheelstop_Material_t
     STF_Parking_Wheelstop_Width_t
     Security Rating (SR1 SR2)
     Sub Discipline Title - Third
     UTSEquipmentCategories
     Unit Type
     View
     Wall_Special Finish
     Warranty Duration (Years)

### SP's using weird characters

	Primary Pump Flow  for 11°C
	Copyright ©
	Plan swing_90°_i
	Plan swing_30°_i
	Plan swing_180°_Offset from wall_i
	Plan swing_45°_i
	DO NOT EDIT_Stacking_Plan rep_90°within opening_Visible_t
	DO NOT EDIT_Stacking_Plan rep_90°beyond opening_Visible_i
	DO NOT EDIT_Stacking_Plan rep_90°beyond opening_Visible_t
	DO NOT EDIT_Stacking_Plan rep_180°_Visible_t
	Plan swing_180°_i
	WB STANDARD don't change
	Plan swing_Double acting_90°_i

[familyParametersCode]: https://github.com/annisarivera/mastercontent/blob/master/working/Master%20Content%20-%20FamilyParameters.ipynb
