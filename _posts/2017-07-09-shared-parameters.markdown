---
layout: post
title:  Shared Parameters
date:   2017-06-14 12:10:13 +1000
categories: jekyll update
assetfolder: familyparameters
# ![png](output_17_0.png)
#to
#![png]({{site.baseurl}}/assets/{{page.assetfolder}}/output_17_0.png)

---

### [Link to the code][sharedParametersCode]

The BVN shared parameters are a list of definitions that can be added to Revit families or projects. 

![png]({{site.baseurl}}/assets/{{page.assetfolder}}/diagram.png)

### GENERAL THINGS ABOUT BVN'S SHARED PARAMETER LIST

There is a total of **427 shared parameters** in this list.

<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: left;">
      <th>BVNSPNAME</th>
      <th>BVNSPGROUP</th>
    </tr>
  </thead>
  <tbody style="text-align: left;">
    <tr>
      <th>01_Annotations</th>
      <td>13</td>
    </tr>
    <tr>
      <th>02_Areas</th>
      <td>22</td>
    </tr>
    <tr>
      <th>03_Casework &amp; Joinery</th>
      <td>61</td>
    </tr>
    <tr>
      <th>04_Ceilings</th>
      <td>5</td>
    </tr>
    <tr>
      <th>05_Curtain Panels</th>
      <td>2</td>
    </tr>
    <tr>
      <th>06_Curtain Walls</th>
      <td>1</td>
    </tr>
    <tr>
      <th>07_Detail Items</th>
      <td>1</td>
    </tr>
    <tr>
      <th>08_Doors</th>
      <td>62</td>
    </tr>
    <tr>
      <th>12_Furniture</th>
      <td>7</td>
    </tr>
    <tr>
      <th>16_Mass</th>
      <td>1</td>
    </tr>
    <tr>
      <th>18_Multiple Categories</th>
      <td>43</td>
    </tr>
    <tr>
      <th>19_Parking</th>
      <td>3</td>
    </tr>
    <tr>
      <th>20_Planting</th>
      <td>1</td>
    </tr>
    <tr>
      <th>21_Plumbing</th>
      <td>5</td>
    </tr>
    <tr>
      <th>24_Rooms</th>
      <td>13</td>
    </tr>
    <tr>
      <th>26_Speciality Equipment</th>
      <td>1</td>
    </tr>
    <tr>
      <th>27_Structural Columns</th>
      <td>6</td>
    </tr>
    <tr>
      <th>29_Structural Framing</th>
      <td>1</td>
    </tr>
    <tr>
      <th>31_Titleblocks</th>
      <td>73</td>
    </tr>
    <tr>
      <th>32_Walls</th>
      <td>9</td>
    </tr>
    <tr>
      <th>33_Windows</th>
      <td>24</td>
    </tr>
    <tr>
      <th>34_Marketing Drawings</th>
      <td>17</td>
    </tr>
    <tr>
      <th>Codebook</th>
      <td>7</td>
    </tr>
    <tr>
      <th>Exported Parameters</th>
      <td>3</td>
    </tr>
    <tr>
      <th>Sefaira Shared Parameters</th>
      <td>2</td>
    </tr>
    <tr>
      <th>Superseeded</th>
      <td>15</td>
    </tr>
    <tr>
      <th>drofus</th>
      <td>23</td>
    </tr>
    <tr>
      <th>drofus instance parameters</th>
      <td>6</td>
    </tr>
  </tbody>
</table>
</div>

<br />

This list has been accumulated and built up over the last few years, though with little organisation and care. Things that contribute to the bad organisation of the list:

- Spelling mistakes
- Duplicates with similar names
- Redundant group naming of parameters (groups that have no parameters in them)
- Ambiguous naming of parameters

For example, there is a parameter called width and width_bvn. Whilst these parameters may seem to have a slight difference in its name, it can cause significant impacts to the revit family or project with scheduling and maintenence in general. 

There needs to be a clean up of this list. However, breaking families and projects that have particular shared parameters is something we do not want to do. 

Therefore, the following information is basically letting us know what BVN shared parameters are being used in both our master content and BVN's Revit project template. 

### MASTER CONTENT SHARED PARAMETERS

#### Cross-checking of shared parameters in master content

The following table determines whether each ** parameter ** of each family in the master content is part of BVN's shared parameter list. If the parameter matches what is coming from the list, the column 'BVNparam' will be true, if not, will show false.

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

#### Number of parameters that are using SP vs non-SP

![png]({{site.baseurl}}/assets/{{page.assetfolder}}/output_28_0.png)

#### Filters for Families that are only using shared parameters

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

#### No. of SP parameters vs non-BVN SP parameters of each family

<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: left;">
      <th></th>
      <th></th>
      <th>ParameterName</th>
    </tr>
    <tr>
      <th></th>
      <th></th>
      <th>count</th>
    </tr>
    <tr>
      <th>FamilyName</th>
      <th>BVNparam</th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th rowspan="2" valign="top">1 Bay Window</th>
      <th>False</th>
      <td>58</td>
    </tr>
    <tr>
      <th>True</th>
      <td>10</td>
    </tr>
    <tr>
      <th rowspan="2" valign="top">1 Bay Window - Non Hosted</th>
      <th>False</th>
      <td>54</td>
    </tr>
    <tr>
      <th>True</th>
      <td>6</td>
    </tr>
    <tr>
      <th>10P_Perimeter_Bench_FYS</th>
      <th>False</th>
      <td>17</td>
    </tr>
  </tbody>
</table>
</div>


<br />

#### SP's that are not used (dead parameters)

** This list is basically (BVN's shared parameter list - list of unique parameters in master content)** 

    01_Lot Number
	02_Lot Number
	03_Lot Number
	04_Lot Number
	05_Lot Number
	06_Lot Number
	07_Lot Number
	08_Lot Number
	09_Lot Number
	10_Lot Number
	11_Lot Number
	12_Lot Number
	13_Lot Number
	14_Lot Number
	15_Lot Number
	16_Lot Number
	A3 Scale
	Acoustic Performance
	Acoustic Rating Rw
	Acoustic Rating Rw/Rw+Ctr
	Adapt_Text
	Adaptable
	Additional Info- Fourth Line
	Apartment Area
	Apartment Number
	Apartment_External Area
	Area Actual vs Briefed
	Area Actual vs Briefed%
	Area Per Occupant
	Area Type
	Area_Briefed
	Aspect
	BVN_API
	Balcony Area
	Balcony Compliance
	Base Name
	Base Number
	Briefed Number of Rooms
	Building Number
	Carpark Allocation
	Ceiling Acoustic Rating
	Ceiling Finish
	Ceiling Finish Colour
	Client Project Number
	Configured By
	Construction
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
	Consultant 06
	Consultant 06 Details
	Consultant 07
	Consultant 07 Details
	Consultant 08
	Consultant 08 Details
	Consultant 09
	Content
	Department Code
	Discipline
	Door Remarks
	Door Type Description
	Door Type Number
	Drawing Revision
	Drawing Scale
	Ext.
	File Type
	Filled Region Area
	Finish on Pull Side
	Finish on Push Side
	Functional Location: Apartment - Number
	Functional Location: Base/ Component - Name
	Functional Location: Building  - Name
	Functional Location: Precinct / Unit - Name
	Functional_Group
	Glazing Type
	Hardware Set
	Htmlink
	Ignore for Sefaira
	Issued to
	Leaf Type
	Level
	Level - Second Line
	Lining_'Opposite Side'
	Lining_'Placement Side'
	Material Sash Glazing
	Member_Length
	Modifiedissue
	Name and Numbers: Room ID
	Name and Numbers: Room Name
	Natspec Section Code
	Natural Cross Ventilation
	Natural Kitchen Ventilation
	Nts
	Number Of Bedrooms
	Package
	Parking_Clearance_Height
	Partition Code
	Partition System Build-up
	Partition System Manufacturer's Code
	Project Manager
	Project Manager'S Details
	Project Name Phase 2
	Project Phase
	Project Status
	Project Status Phase 2
	Project Type
	RDS_Code
	RDS_Description
	RDS_Discipline
	Reference
	Required Area
	Revision Comments
	Revision Date
	Revision Description
	Room Function Number
	Room_Label
	SEPP 65 Solar Access Min 1.75Hrs
	SEPP65_Cross Ventilation
	SEPP65_Solar Access
	SEPP65_South Facing
	Scale Bar 1-1
	Scale Bar 1-10
	Scale Bar 1-100
	Scale Bar 1-1000
	Scale Bar 1-2
	Scale Bar 1-20
	Scale Bar 1-200
	Scale Bar 1-2000
	Scale Bar 1-250
	Scale Bar 1-5
	Scale Bar 1-50
	Scale Bar 1-500
	Scale Printed
	Scale_1
	Scale_2
	Scale_3
	Scalenumber1
	Sequence Number
	Shading for Sefaira
	Sheet Prefix
	Sheet Size
	Solar Access Private Open Space_Min 3 Hrs
	Solar Access_Min 2 Hrs
	Solar Access_Min 3 Hrs
	Sorting Levels
	South Facing
	Spec Description
	State
	State Code
	Strata Area
	Strata Lot Area
	Strata Lot Number
	Subdepartment
	Tbc_Sheet 01
	Tbc_Sheet 02
	Test Adaptable
	Thermal Value
	To be modelled
	Tree Status
	UniqueID
	Unit Name
	Unit Number
	View
	View Fitness
	Vision Panel Type
	Window Performance Type
	article_id
	bim id
	colour
	dRofus Id
	dRofus Item name
	dRofus Item no
	drofus_id
	drofus_occurrence_id
	i-depth
	i-height
	i-length
	item name
	item number
	main group name
	main group number
	model_name_drofus
	name on drawing
	occurrence_id
	room function number
	room number
	room_id
	sub group name
	sub group number
	t-depth
	t-height
	t-length

### PROJECT SHARED PARAMETERS

What was found was that some shared parameter elements was in the BVN revit template. Whilst these parameters were visibly 'deleted' off the template, its remaining information was still hiding in the template. This caused problems when needing to add shared parameters into your project. 

For example, if there was shared parameter called width lurking pre-loaded into the template, and you wanted to add a parameter called WIDTH. Revit would freak out as there are two parameters with the same name but with different letter cases.

But of course, we don't want to delete anything that could cause anything to break. 

Therefore, the following information will show you what hiding shared parameters should be deleted and what can stay in the template.

#### Dead shared parameters in BVN Revit template

This is a list that tells you what can be deleted off the BVN template

**(BVN's shared parameter list - list of shared parameters in the BVN revit template)** 

	AS1428 Tolerance
	AS1482 Tolerance
	Area Colour
	Area_Colour_Bvn
	Armpad Finish
	Asset Number
	Author
	BVN Alphabet
	Back Finish
	Bars
	Base Finish
	Base Price
	Bench_Material_Bvn
	Bench_Thickness_Bvn
	Benchtop Material
	Benchtopfinish
	Benchtopmaterial
	Benchtopthickness
	Bolt Latch
	Briefed Area
	Building Name
	Carcase Offset off Wall
	Carcasefinish
	Carcasematerial
	Carcass Material
	Carcass_Material_Bvn
	Carcess_Thickness_Bvn
	Caseworkoveralldepth
	Caseworkoverallheight
	Caseworkoverallwidth
	Catalog
	Catalog Code
	Category Color
	Cb Classification
	Cb Code 1
	Cb Description
	Cb Group
	Cdeb_Doorid
	Cdeb_Rminstid
	Cdeb_Status
	Ceiling_Height_Bvn
	Cf_1
	Cf_2
	CheckedBy_ANZRS
	Clear Opening
	Closer
	Column Length
	Copyright
	Copyright \xc2\xa9
	Core
	Core Name
	CreatedByURL_ANZRS
	CreatedBy_ANZRS
	DAF_Created By_Username_t
	DAF_Modified By_Username_t
	DAF_Modified_Date_t
	DAF_Owned By_t
	DAF_Revision number_t
	Department_BVN
	Depth_Bvn
	Depth_Two_Bvn
	Detailedcategory
	Door Grille/Undercut
	Door Leaf Height
	Door Leaf Thickness
	Door Leaf Type
	Door Leaf Width
	Door Panel Height
	Door Panel Thickness
	Door Seals
	Door Stop
	Door Thickness
	Door Undercut
	Double Rebate
	Double Swing
	Either Side Swing Away
	Either Side Swing Towards
	Electric Locking
	Electromagnetic Hold Open
	End Panel Side I Finish
	End Panel Side II Finish
	Expected Lifespan (Years)
	Ext Frame_Offset EQUAL Host Wall thickness_i
	FF&E Code
	FF&E Comments
	FF&E Description
	FF&E Group
	FF&E Issue
	FF&E Item
	FF&E Supplier
	FF_SPECIFIC_1
	Ff_1
	Ff_2
	Fire/Smoke Door
	Flux Id
	Frame Finish
	Frame Overlaps Wall
	Frame Profile
	Frame to Match Wall Thickness
	Front Panel Finish
	Front Swing Away
	Front Swing Towards
	Frontpanel_Left_Material_Bvn
	Frontpanel_Right_Material_Bvn
	Frontpanel_Single_Material_Bvn
	Generic Room Sheet Reference
	Glazing
	Glazing Material
	Grade
	Grid Prefix
	Handle Height
	Handle Offset
	Head Details
	Height_Bvn
	Height_Skirting_Bvn
	Height_Two_Bvn
	Hfbs_Sub_Department
	Hinge Side Swing Away
	Hinge Side Swing Towards
	HsbType
	Ideate BIMLink
	ItemCode
	ItemCode_2
	ItemDescription
	ItemDescription_2
	ItemGroup
	ItemGroup_2
	Jamb Details
	Kicker Material
	Kickerfinish
	Kickerheight
	Kickermaterial
	Latch Side Swing Away
	Latch Side Swing Towards
	Leaf 1 Width
	Leaf 2 Width
	Leaf Height
	Length
	Lining_"Opposite Side"
	Lining_"Placement Side"
	Link_Status
	Lock/Latch
	MOUNTING_HEIGHT_US_BVN
	Maintenance Schedule (Months)
	Mass per m
	Material Door Panel
	Material Door Panel EXT
	Material Door Panel INT
	Material Frame
	Material View Panel
	Meeting Stile Detail
	Modified Issue
	ModifiedIssue
	Mounted_Top_Bvn
	Mounting_Height_Bvn
	Mounting_Height_Centre_Bvn
	Mounting_Height_Top_Bvn
	Mullion Height
	No. of Parks
	Original Model By
	Other Protection
	Overall_Height_Bvn
	Package Qty
	Panel 1 Height
	Panel 1 Width
	Panel Height
	Panel Width
	Place in Structural Wall_i
	Product Documentation Link
	Project
	Project Managers Details
	Project Stage
	Project Stage Code
	Protection on Pull Side
	Protection on Push Side
	Pull Handle
	Pull Side Finish Zone
	Push Plates
	Push Side Finish Zone
	Radius
	Reed Switch
	Revision
	Roller Catch
	Room Code
	Room Colour
	Room Name
	SEPP 65 - Cross Ventilation
	SEPP 65 - Solar Access
	SEPP 65 - South Aspect
	SEPP65 - Daylight Access
	SR Document GUID
	SR View Calculation Settings
	STF_ParkingBay_Depth_t
	STF_ParkingBay_Width_t
	STF_Parking_BayAngle_t
	STF_Parking_Disabled_YesNo_t
	STF_Parking_Stripe_End_i
	STF_Parking_Wheelstop_Depth_t
	STF_Parking_Wheelstop_Height_t
	STF_Parking_Wheelstop_Material_t
	STF_Parking_Wheelstop_Position_t
	STF_Parking_Wheelstop_Width_t
	STF_Parking_Wheelstop_YesNo_t
	Seat/Back Fabric
	Security Rating (SR1 ,SR2)
	Side I Divider Panel
	Side I End Panel
	Side I End Panel Extend Back
	Side I Kickplate Flush
	Side I Shadow Margin
	Side II Divider Panel
	Side II End Panel
	Side II End Panel Extend Back
	Side II Kickplate Flush
	Side II Shadow Margin
	Sill Details
	Small Panel Width
	Sp_Area_Designed
	Sp_Ceiling_Height
	Sp_Circulation_Area
	Sp_Comments
	Sp_Department
	Sp_Depth
	Sp_Gfa_Factor
	Sp_Material_Ceilings
	Sp_Material_Walls
	Sp_Net_Area
	Sp_Per_Unit_Area
	Sp_Room_Name
	Sp_Room_Number
	Sp_Total_Gfa_Area
	Sp_Unique_Id
	Sp_Units
	Sp_Width
	Special Hardware
	Stage
	Structural Opening
	Structural Opening Height
	Sub Discipline Title - Third
	Sub-Department
	Swing Angle
	Thickness_Shelf
	UTSEquipmentCategories
	Unit Type
	View Panel
	View Panel Height
	View Panel Inset
	View Panel Sill
	View Panel Width
	WNF_Ext Frame_Offset_Internal Skin_i
	WNF_Frame_Surround_Depth_t
	WNF_Frame_Surround_Width_t
	WNF_Overall Frame Height_t
	WNF_Overall Frame Width_t
	WNF_Panel_Main Fixed_Height_t
	WNF_Panel_Main Fixed_Width_t
	WNP_Schedule Filter_Louvre_t
	Wall_Special Finish
	Warranty Duration (Years)
	Watermarked By
	Wf_E_1
	Wf_E_2
	Wf_N_1
	Wf_N_2
	Wf_S_1
	Wf_S_2
	Wf_W_1
	Wf_W_2
	Width_Bvn
	Width_Corner_Bvn
	Width_Counter_Dda_Bvn
	Width_Two_Bvn
	Window Blind Type
	Window Jockey Sash
	Window Louvre
	Window Shade Centre
	Window Shade Left
	Window Shade Right
	Window Shade Top
	Windowframefinish
	Windowframematerial
	Windowframetype
	Windowglazingtype
	Windowheadheight
	Windowoverallframeheight
	Windowoverallframewidth
	Y-Tower Finish
	Zone
	_SPEC_WILKHAHN_ANSI/BIFMA_STANDARDS
	_SPEC_WILKHAHN_DIN_EN_STANDARDS
	_SPEC_WILKHAHN_FURNTECH-AFRDI_BLUE_TICK
	_SPEC_WILKHAHN_FURNTECH-AFRDI_GREEN_TICK
	_SPEC_WILKHAHN_GS_SYMBOL
	_SPEC_WILKHAHN_Model
	_SPEC_WILKHAHN_NPR_STANDARDS
	_SPEC_WILKHAHN_Part_Number
	_SPEC_WILKHAHN_Table_Length
	_SPEC_WILKHAHN_Table_Width
	_SPEC_WILKHAHN_URL
	_SPEC_WILKHAHN_Version
	_WILKHAHN Table Height
	_WILKHAHN Table Length
	_WILKHAHN Table Width
	rwcalc_Carcase Inside Width
	rwcalc_Cupboard1 Height
	rwcalc_Double Panel Width
	rwcalc_Front Panel Visibility
	rwcalc_Kickplate On
	rwcalc_Kickplate Side I setback
	rwcalc_Kickplate Side II setback
	rwcalc_Kickplate Visibility
	rwcalc_Panel Back Offset
	rwcalc_Panel Inset Side I
	rwcalc_Panel Inset Side II
	rwcalc_Panel Offset off Base
	rwcalc_Panel Thk Base
	rwcalc_Panel Thk Side I
	rwcalc_Panel Thk Side II
	rwcalc_Panel Thk Top
	rwcalc_Rail Offset
	rwcalc_Rail1
	rwcalc_Rail2
	rwcalc_Real Panel Base Thk
	rwcalc_Real Panel Side I Thk
	rwcalc_Real Panel Side II Thk
	rwcalc_Real Panel Top Thk
	rwcalc_Shelf Depth
	rwcalc_Shelf1
	rwcalc_Shelf2
	rwcalc_Shelf2 Height
	rwcalc_Shelf3
	rwcalc_Shelf3 Height
	rwcalc_Shelf4
	rwcalc_Shelf4 Height
	rwcalc_Shelf5
	rwcalc_Shelf5 Height
	rwcalc_Shelf6
	rwcalc_Shelf6 Height
	rwcalc_Show Double Front Panel
	rwcalc_Show Single Front Panel
	rwcalc_Single Panel Width
	rwcalc_Swappable
	rwcalc_Symbolic Dept

#### OTHER COMMENTS ABOUT BVN'S SHARED PARAMETER LIST

This is ist of the redundant groups in the BVN shared parameter list (groups that have no parameters in them).

	09_Electrical
	10_Entourage
	11_Floors
	13_Furniture Systems
	14_Generic Models
	15_Lighting
	17_Mechanical 
	22_Profiles
	23_Railings
	25_Site
	28_Structural Foundations
	30_Telephone Device


[sharedParametersCode]: https://github.com/annisarivera/mastercontent/blob/master/working/Master%20Content%20-%20FamilyParameters.ipynb