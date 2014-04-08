|Authoring Program(Version,Element)|Export Program(Version,MVD)|Import Program(Version,MVD)|Data Translation|Notes...............................................|                   
| --- | --- | --- | ------------------- | -------------- |
|Revit(2014,Filled_Region(Draft))|IFCExporter(2_9_0,FMHO)|Revit(2014,Default)|Partial|'Draft File Pattern' changes to 'Model Fill Pattern'
|Revit(2014,Model_Line)|IFCExporter(2_9_0,FMHO)|Revit(2014,Default)|Yes|
|Revit(2014,Model_Line)|IFCExporter(2_9_0,CV_2_0)|Revit(2014,Default)|No|'Model Line' missing
|Revit(2014,Text_Notes)|IFCExporter(2_9_0,FMHO)|Revit(2014,Default)|Yes|3 different scales translated, as well.
|Revit(2014,Text_Notes)|IFCExporter(2_9_0,CV_2_0)|Revit(2014,Default)|No|Missing
|Revit(2014,Wall(Base_Constraint('Level 1'),Top_Constraint('Level 2'))|IFCExporter(2_9_0,CV_2_0)|Revit(2014,Default)|Partial|'Top Constraint' = Unconnected
|Revit(2014,Wall(Edit_Profile('Square Opening')))|IFCExporter(2_9_0,CV_2_0)|Revit(2014,Default)|Partial|('Opening Profile' is missing, New 'Rectangular Straight Wall Opening' Object created)
|Revit(2014,Wall(Edit_Profile('Top Arc')))|IFCExporter(2_9_0,CV_2_0)|Revit(2014,Default)|No|No longer an intelligent wall object--reduced to an in-place family
|Revit(2014,Wall(Edit_Profile('Top Cant')))|IFCExporter(2_9_0,CV_2_0)|Revit(2014,Default)|Partial|Modified profile reset, new IFCOpeningElements used to create 'void'.
|Revit(2014,Wall(Rectangular_Straight_Wall_Opening(Base_Constraint('Level 1'),Top_Constriant('Level 2')))|IFCExporter(2_9_0,CV_2_0)|Revit(2014,Default)|Partial|'Top Constraint' went from 'Level 2' to 'Level 1'.
|Revit(2014,Wall(Rectangular_Straight_Wall_Opening(Base_Constraint('Level 1'),Top_Constriant('Level 1')))|IFCExporter(2_9_0,CV_2_0)|Revit(2014,Default)|Yes|
|Revit(2014,Wall(Walls_Joins(Butt(Dont_Clean_Join))))|IFCExporter(2-9_0,CV_2_0)|Revit(2014,Default)|No|
|Revit(2014,Wall(Walls_Joins(Clean)))|IFCExporter(2_9_0,CV_2_0)|Revit(2014,Default)|Yes|Default 'join' in Revit
|Revit(2014,Wall(Walls_Joins(Miter(Dont_Clean_Join))))|IFCExporter(2-9_0,CV_2_0)|Revit(2014,Default)|No|
