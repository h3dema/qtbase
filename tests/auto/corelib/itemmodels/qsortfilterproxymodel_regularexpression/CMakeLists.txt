# Generated from qsortfilterproxymodel_regularexpression.pro.

#####################################################################
## tst_qsortfilterproxymodel_regularexpression Test:
#####################################################################

add_qt_test(tst_qsortfilterproxymodel_regularexpression
    SOURCES
        ../../../other/qabstractitemmodelutils/dynamictreemodel.cpp ../../../other/qabstractitemmodelutils/dynamictreemodel.h
        ../qsortfilterproxymodel_common/tst_qsortfilterproxymodel.cpp ../qsortfilterproxymodel_common/tst_qsortfilterproxymodel.h
        tst_qsortfilterproxymodel_regularexpression.cpp
    INCLUDE_DIRECTORIES
        ../../../other/qabstractitemmodelutils
        ../qsortfilterproxymodel_common
    PUBLIC_LIBRARIES
        Qt::Gui
        Qt::Widgets
)
