# Status-of-World-Soil-Resources---Southern-Mexico-Central-America-and-the-Caribbean
Supplementary dataset of the chapter published by FAO
Authors:

- Luis Felipe Castelblanco Rivera, master student in Earth Science at Geosciences Center, UNAM.

- Mario Antonio Guevara Santamaría, associate professor at Geosciences Center, UNAM campus Juriquilla 

.

More information:

- lcastelblancor@geociencias.unam.mx / lfcastelblancor@unal.edu.co

- mguevara@geociencias.unam.mx / mguevara@comunidad.unam.mx

Abstract:

This chapter thoroughly examines soil threats and trends in Southern Mexico, Central America, and the Caribbean, emphasizing their implications for sustainable land management. Through a comprehensive analysis of available data and literature, the study identifies erosion patterns, soil carbon changes, soil biodiversity indicators, nutrient mismanagement, salinization, sodification, and soil moisture decline as prominent concerns. Erosion is a significant issue, exacerbated by bare soil conditions, coastal erosion due to rising sea levels, and wind erosion influenced by land use and vegetation cover. Soil carbon changes exhibit both sequestration and loss patterns, particularly impacting agricultural soils, while soil biodiversity's role in nutrient cycling underscores the need for enhanced preservation efforts. Nutrient mismanagement, exemplified by fertilizer consumption trends and efficiency, underscores the importance of informed decision-making in optimizing soil fertility. In response to human activities, soil salinization and sodification significantly threaten agricultural sustainability, particularly across coastal areas. Soil moisture decline, linked to land use intensification and extreme climate events, further exacerbates soil degradation risks. The chapter concludes by advocating for comprehensive soil monitoring and management strategies to address these threats, which are crucial for safeguarding soil health, preserving ecosystem services, and ensuring long-term food security in the region.

Folder description:

-> SoWSR_SMx_CA_Crb.7z
	-> extent
		- Extent_AOI_Union.shp 				#Country boundaries
		- Modis_CLC.shp 				#Corine Land Cover from MODIS
		- WRBpol.shp 					#Most probable soil type using WRB classification
		- Extent_level3.shp 				#Intersection of previous Shapes
	-> level3 						#This folder contains the data frame results of calculating zonal statistics from the rasters.
		- Bare_1km_km2_ZonalStats.csv 			
		- CIC_0-30cm_ZonalStats.csv 			
		- CN_ratio_SoilGrids_null_ZonalStats.csv 	
		- GSOCmap1.5.0_ZonalStats.csv 			
		- GSOCseq_absolute_ZonalStats.csv 
		- GSOCseq_RSR_SSM1_Map030_ZonalStats.csv
		- level3_merged.csv
		- N_0-30cm_ZonalStats.csv
		- Rs_slope_sig_negative_ZonalStats.csv
		- Rs_slope_sig_positive_ZonalStats.csv
		- Salinidad_problema_ZonalStats.csv
		- SM_slope_negative_ZonalStats.csv
		- SM_slope_positive1_ZonalStats.csv
		- SOC_slope_negative_ZonalStats.csv
		- SOC_slope_positive1_ZonalStats.csv
		- SOCDensity_0_30cm_ZonalStats.csv
	-> rasters
		- Bare_1km_km2.tif				#Bare soil percent per square kilometer
		- CIC_0-30cm.tif				#Cation exchange capacity in mmolc/kg
		- CN_ratio_SoilGrids_null			#Carbon:Nitrogen ratio from the report of SoilGrids
		- GSOCmap1.5.0.tif				#Stock of global soil carbon reported by FAO 
		- GSOCseq_absolute.tif				#Product of the difference between initial stock of GSOCmap and Final Stock SSM1 from FAO 
		- GSOCseq_RSR_SSM1_Map030.tif			#Relative Sequestration Rates SSM1 from FAO
		- N_0-30cm					#Soil nitrogen content in cg/kg
		- Rs_slope_sig_negative.tif			#Heterotrofic respiration negative trend
		- Rs_slope_sig_positive.tif			#Heterotrofic respiration positive trend
		- Salinidad_problema.tif			#Areas with salinity (>3 ds/m) from https://doi.org/10.1016/j.rse.2019.111260
		- SM_slope_negative.tif				#Soil moisture negative trend from https://doi.org/10.5194/essd-14-4473-2022
		- SM_slope_positive1.tif			#Soil moisture positive trend from https://doi.org/10.5194/essd-14-4473-2022
		- SOC_slope_negative.tif			#Soil organic carbon negative trend from https://doi.org/10.5067/3K9F0S1Q5J2U
		- SOC_slope_positive1.tif			#Soil organic carbon positive trend from https://doi.org/10.5067/3K9F0S1Q5J2U
	- DB_final.xlsx 					#Data base with the information extract from de raster to build the quantitative data presented in the chapter
	- ZonalStat_for_prl.py 					#Python script to process the zonal statictis of the rasters using the extent (Shapes) to obtain the data frames (CSV) in folder level3.
