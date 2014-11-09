ADD_EXECUTABLE(tspatial EXCLUDE_FROM_ALL ./tspatial.cpp)
PKG_CONFIG_USE_DEPENDENCY(tspatial eigen3)

ADD_EXECUTABLE(symmetric EXCLUDE_FROM_ALL ./symmetric.cpp)
PKG_CONFIG_USE_DEPENDENCY(symmetric eigen3)

ADD_EXECUTABLE(constraint EXCLUDE_FROM_ALL ./constraint.cpp)
PKG_CONFIG_USE_DEPENDENCY(constraint eigen3)

ADD_EXECUTABLE(rnea EXCLUDE_FROM_ALL ./rnea.cpp)
PKG_CONFIG_USE_DEPENDENCY(rnea eigen3)

ADD_EXECUTABLE(crba EXCLUDE_FROM_ALL ./crba.cpp)
PKG_CONFIG_USE_DEPENDENCY(crba eigenpy) # Should be eigen3 as well. Problem of link with ROS.
PKG_CONFIG_USE_DEPENDENCY(crba urdfdom)

ADD_EXECUTABLE(jacobian EXCLUDE_FROM_ALL ./jacobian.cpp)
PKG_CONFIG_USE_DEPENDENCY(jacobian eigen3)

ADD_EXECUTABLE(com EXCLUDE_FROM_ALL ./com.cpp)
PKG_CONFIG_USE_DEPENDENCY(com eigen3)

ADD_EXECUTABLE(cholesky EXCLUDE_FROM_ALL ./cholesky.cpp)
PKG_CONFIG_USE_DEPENDENCY(cholesky eigen3)
PKG_CONFIG_USE_DEPENDENCY(cholesky urdfdom)

ADD_EXECUTABLE(urdf EXCLUDE_FROM_ALL ./urdf.cpp)
PKG_CONFIG_USE_DEPENDENCY(urdf eigen3)
PKG_CONFIG_USE_DEPENDENCY(urdf urdfdom)

ADD_EXECUTABLE(value EXCLUDE_FROM_ALL ./value.cpp)
PKG_CONFIG_USE_DEPENDENCY(value eigen3)
PKG_CONFIG_USE_DEPENDENCY(value urdfdom)

ADD_EXECUTABLE(variant EXCLUDE_FROM_ALL ./variant.cpp)
PKG_CONFIG_USE_DEPENDENCY(variant eigen3)