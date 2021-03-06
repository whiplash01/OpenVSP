CMAKE_MINIMUM_REQUIRED(VERSION 2.8)

SET(GEOM_CORE_INCLUDE_DIR ${CMAKE_CURRENT_SOURCE_DIR} CACHE PATH "Path to geom_core headers")

INCLUDE_DIRECTORIES( 
    ${ANGELSCRIPT_INCLUDE_DIR}
    ${ANGELSCRIPT_ADD_ON_INCLUDE_DIR}
    ${UTIL_INCLUDE_DIR}
    ${CPPTEST_INCLUDE_DIRS} 
    ${LIBXML2_INCLUDE_DIR}
    ${XMLVSP_INCLUDE_DIR}
    ${TRIANGLE_INCLUDE_DIR}
    ${NANOFLANN_INCLUDE_DIR}
    ${CLIPPER_INCLUDE_DIR}
    ${EIGEN3_INCLUDE_DIR}
    ${CodeEli_INCLUDE_DIRS}
    ${TRITRI_INCLUDE_DIR}
    ${PROJECT_SOURCE_DIR}/geom_api
    ${GEOM_API_INCLUDE_DIR}
    ${CMINPACK_INCLUDE_DIR}
    ${STEPCODE_INCLUDE_DIR}
    ${LIBIGES_INCLUDE_DIR}
    ${WAVEDRAGEL_INCLUDE_DIR}
   )

ADD_LIBRARY(geom_core
AdvLink.cpp
AdvLinkMgr.cpp
Airfoil.cpp
AnalysisMgr.cpp
BlankGeom.cpp
CfdMeshSettings.cpp
ClippingMgr.cpp
CustomGeom.cpp
DegenGeom.cpp
DesignVarMgr.cpp
FitModelMgr.cpp
FuselageGeom.cpp
Geom.cpp
GeomCoreTestSuite.cpp
GridDensity.cpp
GroupTransformations.cpp
HingeGeom.cpp
Link.cpp
LinkMgr.cpp
MaterialMgr.cpp
MeshGeom.cpp
Parm.cpp
ParmContainer.cpp
ParmMgr.cpp
ParmUndo.cpp
PCurve.cpp
PodGeom.cpp
ProjectionMgr.cpp
PropGeom.cpp
PtCloudGeom.cpp
ResultsMgr.cpp
ScriptMgr.cpp
SnapTo.cpp
StackGeom.cpp
SubSurface.cpp
SubSurfaceMgr.cpp
Texture.cpp
TextureMgr.cpp
TMesh.cpp
VarPresetMgr.cpp
Vehicle.cpp
VehicleMgr.cpp
WaveDragMgr.cpp
WingGeom.cpp
XSec.cpp
XSecCurve.cpp
XSecSurf.cpp
Label.cpp
LabelMgr.cpp
Light.cpp
LightMgr.cpp
Color.cpp
ColorMgr.cpp
VSPAEROMgr.cpp
AdvLink.h
AdvLinkMgr.h
Airfoil.h
AnalysisMgr.h
BlankGeom.h
CfdMeshSettings.h
ClippingMgr.h
Color.h
ColorMgr.h
CustomGeom.h
DegenGeom.h
DesignVarMgr.h
DragFactors.h
FitModelMgr.h
FuselageGeom.h
Geom.h
GeomCoreTestSuite.h
GridDensity.h
GroupTransformations.h
HingeGeom.h
Label.h
LabelMgr.h
Light.h
LightMgr.h
Link.h
LinkMgr.h
MaterialMgr.h
MeshGeom.h
Parm.h
ParmContainer.h
ParmMgr.h
ParmUndo.h
PCurve.h
PodGeom.h
ProjectionMgr.h
PropGeom.h
PtCloudGeom.h
ResultsMgr.h
ScriptMgr.h
SnapTo.h
StackGeom.h
SubSurface.h
SubSurfaceMgr.h
SWIGDefines.h
Texture.h
TextureMgr.h
TMesh.h
VarPresetMgr.h
Vehicle.h
VehicleMgr.h
VSPAEROMgr.h
WaveDragMgr.h
WingGeom.h
XSec.h
XSecCurve.h
XSecSurf.h
)

ADD_DEPENDENCIES( geom_core
util
)
