# webapp_ANPR
Phase 1: collect and annotate images


collect images of vehicle number plate 
download labelimg
  Labelimg is a GUI based image annotation application which help to annotate vehicle number plate
 
 using Labelimg Gui interface create .xml extention file. 
        what is inside .xml?
          This is the file which is created while you annotate vehicle number plate using GUI based Labelimg.
         
following is one of the .xml file 

<annotation>
	<folder>images</folder>
	<filename>N103.jpeg</filename>
	<path>/home/captain/Desktop/webapp/images/N103.jpeg</path>
	<source>
		<database>Unknown</database>
	</source>
	<size>
		<width>1800</width>
		<height>1200</height>
		<depth>3</depth>
	</size>
	<segmented>0</segmented>
	<object>
		<name>number_plate</name>
		<pose>Unspecified</pose>
		<truncated>0</truncated>
		<difficult>0</difficult>
		<bndbox>
			<xmin>819</xmin>
			<ymin>685</ymin>
			<xmax>1064</xmax>
			<ymax>734</ymax>
		</bndbox>
	</object>
</annotation>

After completion of annotating image sum code on 01_xml_to_csv.ipynb.
This will give you an .csv extension file from .xml

Why .csv instead of .xml?
  pandas dataframe(df) is used to access .csv file which wll be more easier while accessing data into tabular format.
  
After completion of 01_xml_to_csv.ipynb

phase 2: Object detection
