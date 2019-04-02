set(appname CERSN002)

set(scripts CERSN002_all.xml
            yarprobotinterface.ini general.xml yarpmotorgui.ini)

yarp_install(FILES ${scripts} DESTINATION ${CER_ROBOTS_INSTALL_DIR}/${appname})
yarp_install(DIRECTORY calibrators DESTINATION ${CER_ROBOTS_INSTALL_DIR}/${appname})
yarp_install(DIRECTORY wrappers DESTINATION ${CER_ROBOTS_INSTALL_DIR}/${appname})
yarp_install(DIRECTORY hardware DESTINATION ${CER_ROBOTS_INSTALL_DIR}/${appname})

