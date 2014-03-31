|Authoring Program(Version,Element)|Export Program(Version,MVD)|Import Program(Version,MVD)|Data Translation|Notes...............................................|                   
| --- | --- | --- | ------------------- | -------------- |
|Revit(2014,Filled_Region(Draft))|IFCExporter(2_9_0,FMHO)|Revit(2014,Default)|Partial|'Draft File Pattern' changes to 'Model Fill Pattern'
|Revit(2014,Model_Line)|IFCExporter(2_9_0,FMHO)|Revit(2014,Default)|Yes|
|Revit(2014,Model_Line)|IFCExporter(2_9_0,CV_2_0)|Revit(2014,Default)|No|Model_Line missing
|Revit(2014,Text_Notes)|IFCExporter(2_9_0,FMHO)|Revit(2014,Default)|Yes|3 different scales translated, as well.
|Revit(2014,Text_Notes)|IFCExporter(2_9_0,CV_2_0)|Revit(2014,Default)|No|Missing
|Revit(2014,Wall(Base_Constraint('Level 1'),Top_Constraint('Level 2'))|IFCExporter(2_9_0,CV_2_0)|Revit(2014,Default)|Partial|(Top Constraint = Unconnected, IFC Parameters added)
|Revit(2014,Wall('Opening by Edit Profile'))|IFCExporter(2_9_0,CV_2_0)|Revit(2014,Default)|Partial|('Opening Profile' is missing, New 'Rectangular Straight Wall Opening' Object created)