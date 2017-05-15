cmake_minimum_required(VERSION 2.8.9)

project(LabExt)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "http://slicer.org/slicerWiki/index.php/Documentation/Nightly/Extensions/LabExt")
set(EXTENSION_CATEGORY "Examples")
set(EXTENSION_CONTRIBUTORS "Dawid Biela (IwM1)")
set(EXTENSION_DESCRIPTION "Rozszerzenie stworzone na potrzeby laboratorium z PWP")
set(EXTENSION_ICONURL "http://www.example.com/Slicer/Extensions/LabExt.png")
set(EXTENSION_SCREENSHOTURLS "http://www.example.com/Slicer/Extensions/LabExt/Screenshots/1.png")
set(EXTENSION_DEPENDS "NA") # Specified as a space separated string, a list or 'NA' if any

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(Laborka)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_CPACK})
