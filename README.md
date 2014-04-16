# IFC_roundtrip
----------
A open, crowdsourced library of IFC/BIM test files--striving for bi-directional/roundtrip functionality between BIM programs.

----------

Hopefully, in the future, this project will evolve to the point that it could be used, in some capacity, to improve the fidelity of BuildingSmart's [MVD Certifications](http://www.buildingsmart-tech.org/certification).

Initial focus will include Buildingsmart's current MVD releases: 

 - [IFC2x3 Coordination View Version 2.0](http://www.buildingsmart-tech.org/specifications/ifc-view-definition/coordination-view-v2.0) (CV_2_0)
 - [IFC2x3 Structural Analysis View](http://www.buildingsmart-tech.org/specifications/ifc-view-definition/structural-analysis-view) (SAV)
 - [IFC2x3 Basic FM HandOver](http://www.buildingsmart-tech.org/specifications/ifc-view-definition/fm-handover-aquarium) (FMHO)

----------
### Contributing
----------
As it is open source, and crowdsourced, please add to the project as you see fit.  As you can imagine, this is a BIG project.

...

The way i'm tackling it thus far, is to create a native object within a native authoring BIM program that tests one single function/attribute.

examples...

* wall linked/constrained to building elevations
* wall with unique header profile
* slab with a slope
* slab with a opening
* slab with different material profiles/layers
* door with a 2d swing profile
* etc. <the isolated test cases are virtually endless--the idea is to test one thing only.>

The next step is to export out an IFC file using the authoring program's specific MVD settings *(Coordination View 2.0 or FM handover, for example)*

*The idea here, is to test the fidelity of the program's MVD translation, not to tweak the IFC export settings of a particularity BIM program*

The next step is to import the test file into another BIM platform, again using a specific MVD setting. From here, I've denoted that if the translation has passed/failed (or partial) based on how much 'intelligence' remains intact upon import.

Although somewhat vague, *(could use help tightening this definition)*, I define ‘intelligence’ as how easy/hard it would be to re-conjure or imbue the import object with the same functionality that was present in the export program.

I use the following logic for file naming *(a logic that could change over time, open to ideas)*...

* Authoring Program(Version,Element & Test)--Export Program(Version,MVD)--Import Program(Version,MVD)

Examples:

* Revit(2014,Wall(Base_Constraint('Level 1'),Top_Constriant('Level 2'))--IFCExporter(2_9_0,CV_2_0)--ArchiCAD(17,CV_2_0).pln
* ArchiCAD(17,Wall(Home_Link('1st FLOOR'),Top_Link('2nd FLOOR'))--ArchiCAD(17,CV_2_0)--Revit(2014,default).rvt

In terms of help, it would be great to work with other IFC enthusiasts who can either create native/IFC test files from their BIM platform of choice and/or import the IFC files from other platforms, and report results.

As i said before, i expect this project to evolve over time and am open to reinterpretations and reformatting of the approaches. Thus the beauty of open source--please fork at your fancy.

----------
### Tools
----------
If you're not familar with Git or Github workflow, I highly recommend using [Github's Windows Client](https://windows.github.com/).  Go [here](http://windows.github.com/help.html), for an overview.  Once you start using this [distributed revision control](http://en.wikipedia.org/wiki/Distributed_revision_control), you will start demanding similar workflows in the AEC industry. 

----------
### License
----------
Highly permissive!
BSD, MIT... take your pick.
